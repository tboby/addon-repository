# tboby's Add-ons

## About

Home Assistant allows anyone to create add-on repositories to share their
add-ons for Home Assistant easily. This repository is one of those repositories,
providing extra Home Assistant add-ons for your installation.


## Installation

In the Home Assistant add-on store, a possibility to add a repository is provided.

Use the following URL to add this repository:

```txt
https://github.com/tboby/addon-repository
```

## Add-ons provided by this repository

### &#10003; [ONNX ASR][addon-onnx-asr]

![Latest Version][onnx-asr-version-shield]
![Supports aarch64 Architecture][onnx-asr-aarch64-shield]
![Supports amd64 Architecture][onnx-asr-amd64-shield]

Home Assistant add-on that uses onnx-asr for speech-to-text.

Notably, provides access to the NVIDIA NeMo Parakeet-TDT model which should be significantly faster and more accurate than Whisper for English.

[:books: ONNX ASR add-on documentation][addon-doc-onnx-asr]

## Releases

Releases are based on [Semantic Versioning][semver], and use the format
of ``MAJOR.MINOR.PATCH``. In a nutshell, the version will be incremented
based on the following:

- ``MAJOR``: Incompatible or major changes.
- ``MINOR``: Backwards-compatible new features and enhancements.
- ``PATCH``: Backwards-compatible bugfixes and package updates.

## Support

Got questions?

People on the Home Assistant Discord Chat Server may be able to help.

You could also open an issue here on GitHub. Note, there is a separate
GitHub repository for each add-on. Please ensure you are creating the issue
on the correct GitHub repository matching the add-on.

- [Open an issue for the add-on: ONNX ASR][onnx-asr-issue]

For a general repository issue or add-on ideas [open an issue here][issue]

## Acknowledgements

This repository is heavily based upon the hassio addons repository, which is licensed:

MIT License

Copyright (c) 2017-2024 Franck Nijhof

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

[addon-onnx-asr]: https://github.com/tboby/onnx-asr-addon/tree/v0.1.2
[addon-doc-onnx-asr]: https://github.com/tboby/onnx-asr-addon/blob/v5.3.0/onnx-asr/DOCS.md
[onnx-asr-issue]: https://github.com/tboby/onnx-asr-addon/issues
[onnx-asr-aarch64-shield]: https://img.shields.io/badge/aarch64-yes-green.svg
[onnx-asr-amd64-shield]: https://img.shields.io/badge/amd64-yes-green.svg
[onnx-asr-version-shield]: https://img.shields.io/badge/version-v0.1.2-blue.svg

[awesome-shield]: https://img.shields.io/badge/awesome%3F-yes-brightgreen.svg
[awesome]: https://awesome-ha.com
[discord-ha]: https://discord.gg/c5DvZ4e
[discord-shield]: https://img.shields.io/discord/478094546522079232.svg
[discord]: https://discord.me/hassioaddons
[forum-frenck]: https://community.home-assistant.io/u/frenck/?u=frenck
[forum-shield]: https://img.shields.io/badge/community-forum-brightgreen.svg
[forum]: https://community.home-assistant.io?u=frenck
[frenck]: https://github.com/frenck
[gitlabci-shield]: https://gitlab.com/hassio-addons/repository/badges/master/pipeline.svg
[gitlabci]: https://gitlab.com/hassio-addons/repository/pipelines
[issue]: https://github.com/hassio-addons/repository/issues
[license-shield]: https://img.shields.io/github/license/hassio-addons/repository.svg
[maintenance-shield]: https://img.shields.io/maintenance/yes/2025.svg
[project-stage-shield]: https://img.shields.io/badge/project%20stage-production%20ready-brightgreen.svg
[reddit]: https://reddit.com/r/homeassistant
[semver]: http://semver.org/spec/v2.0.0.html
