# Home Assistant Add-on: ONNX ASR

This is a drop-in replacement for the Official Whisper Add-on, providing access to a different set of models.

It may also run certain whisper models faster depending on your CPU.

## ⚠️ Warning—Memory intense in default configuration

It's strongly recommended you only use this Add-on on systems with more than 8GB of RAM.

When configured in auto, the english model uses 2.5GB at all times.

When configured in auto, the multilingual mode uses 2.5GB at all times.

## Installation

Follow these steps to get the add-on installed on your system:

1. Navigate in your Home Assistant frontend to **Settings** -> **Add-ons** -> **Add-on store**..
2. Find the "ONNX ASR" add-on and click it.
3. Click on the "INSTALL" button.

## How to use

After this add-on is installed and running, it will be automatically discovered
by the Wyoming integration in Home Assistant. To finish the setup,
click the following my button:

[![Open your Home Assistant instance and start setting up a new integration.](https://my.home-assistant.io/badges/config_flow_start.svg)](https://my.home-assistant.io/redirect/config_flow_start/?domain=wyoming)

Alternatively, you can install the Wyoming integration manually, see the
[Wyoming integration documentation](https://www.home-assistant.io/integrations/wyoming/)
for more information.

## Configuration

### Option: `model_en`

ONNX ASR model that will be used for English transcription. Choose `custom` to use the model name in `custom_model`, which may be a HuggingFace model ID like "Systran/faster-distil-whisper-small.en".

The default model is `auto`, which selects `nemo-parakeet-tdt-0.6b-v2` for English-only configurations, or `nemo-parakeet-tdt-0.6b-v3` for multi-language configurations.

Available models, english only:

- `auto` (select author's most efficient model)
- `nemo-parakeet-tdt-0.6b-v2`
- `nemo-parakeet-rnnt-0.6b`
- `nemo-parakeet-ctc-0.6b`
- `nemo-canary-1b-v2`
- `onnx-community/whisper-base.en`
- `onnx-community/whisper-tiny.en`
- `onnx-community/whisper-small.en`
- `whisper-base`

### Option: `model_multilingual`

ONNX ASR model that will be used for non-english transcription. Choose `custom` to use the model name in `custom_model`, which may be a HuggingFace model ID like "Systran/faster-distil-whisper-small.en".

The default model is `auto`, which selects `nemo-parakeet-tdt-0.6b-v3` for multi-language configurations, which has slightly worse english performance than v2 but supports a wide range of languages.

Available models:

- `auto` (select author's most efficient model)
- `nemo-parakeet-tdt-0.6b-v3`
- `nemo-canary-1b-v2`
- `whisper-base`
- `onnx-community/whisper-tiny`
- `onnx-community/whisper-base`
- `onnx-community/whisper-small`
- `onnx-community/whisper-large-v3-turbo`

[Performance of supported languages](https://github.com/openai/whisper#available-models-and-languages)

### Option: `custom_model_en`

HuggingFace Hub model ID like "nvidia/stt_en_conformer_ctc_large". Only models supported by onnx-asr will work.

### Option: `custom_model_multilingual`

HuggingFace Hub model ID like "nvidia/stt_en_conformer_ctc_large". Only models supported by onnx-asr will work.

## Backups

Model files can be large, so they are automatically excluded from backups and re-downloaded on restore for remote models.
After restoring a backup with a local custom model, manually copy your model directory again.

## Support

Got questions?

People on the [Home Assistant Discord Chat Server][discord] may be able to help.

In case you've found an bug, please [open an issue on our GitHub][issue].

[discord]: https://discord.gg/c5DvZ4e
[issue]: https://github.com/tboby/wyoming-onnx-asr/issues
[repository]: https://github.com/tboby/wyoming-onnx-asr
