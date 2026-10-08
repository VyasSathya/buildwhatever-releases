# BuildWhatever releases

Windows alpha release distribution for BuildWhatever, an AI-assisted game-editor project. This repository provides release artifacts and usage notes; it does not include the editor's source implementation.

## Download

Use the [latest release](https://github.com/VyasSathya/buildwhatever-releases/releases/latest) or the recorded [v0.2.0-alpha release](https://github.com/VyasSathya/buildwhatever-releases/releases/tag/v0.2.0-alpha).

The release metadata checked on October 8, 2026 records:

| Item | Value |
| --- | --- |
| Release tag | `v0.2.0-alpha` |
| Published | March 23, 2026 |
| Windows x86_64 asset | `buildwhatever-v0.1.0-alpha-windows-x86_64.zip` |
| Archive size | 73,431,125 bytes |
| GitHub-provided SHA-256 | `53cf3e256c17aaca4ec6db923755f748f4f263d85f81c9d2ac1f81508effadd5` |

The asset is a ZIP archive, not the standalone executable previously named in this README. Download and extract the archive to inspect its editor executable and packaged files. The release tag and archive filename use different version labels; they should not be treated as proof of identical package/version metadata.

The digest above comes from GitHub's asset metadata. The archive was not downloaded, independently hashed, or executed during this documentation review.

## AI configuration

The project's earlier usage notes describe an AI Chat dock and provider settings under **Editor > AI Settings**. They describe cloud-provider configuration through OpenRouter and a local Ollama option. Actual availability depends on the packaged release and needs verification in that build.

Provider credentials belong in the editor's local configuration, not in a Git commit. Current model availability, prices, hardware requirements, and feature support are not guaranteed by this release repository.

## Alpha status

The release uses an alpha tag, although GitHub currently marks it as a regular release rather than a prerelease. Windows compatibility, project import/export, AI interactions, and the editor's claimed Godot-fork features have not been validated from this repository's source, because that source is not included.

## Command reference from the project notes

The original editor guide records these AI-chat commands; check their availability in the extracted build:

| Command | Recorded purpose |
| --- | --- |
| `/clear` | Clear chat history |
| `/plan` | Toggle planning mode |
| `/model` | Show the selected model |
| `/export` / `/import` | Save or load a chat session |
| `/help` | List available commands |

Those notes also describe `@` project-file references and an attachment control. No benchmark, API-price estimate, or tested-system claim is made here.

## License and provenance

The project is described in its original notes as a Godot Engine fork. Source-license attribution, third-party notices, and the packaged editor's redistribution terms still need to be documented alongside the artifact. No root license file is included in this repository.
