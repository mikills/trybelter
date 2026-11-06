# Belter

Belter is a design tool. This repository holds the downloads. The source code is not public (yet).

Belter is free, and you do not need an account. The app and the `belter` command-line tool work on your own files,
on your own computer.

## Download

Go to [Releases](https://github.com/mikills/trybelter/releases/latest) and pick the file for your computer.

### The app (macOS)

| File | For |
| --- | --- |
| `Belter-<version>-arm64.dmg` | Apple silicon Macs (M1 and later) |
| `Belter-<version>-x64.dmg` | Intel Macs |

The app needs macOS 12 or later. Open the DMG and drag Belter to Applications.

### The command-line tool

| File | For |
| --- | --- |
| `belter-cli-<version>-macos-arm64.zip` | macOS, Apple silicon |
| `belter-cli-<version>-macos-x64.zip` | macOS, Intel |
| `belter-cli-<version>-linux-arm64.tar.gz` | Linux, ARM 64-bit |
| `belter-cli-<version>-linux-x64.tar.gz` | Linux, x86 64-bit |

On macOS:

```bash
unzip belter-cli-<version>-macos-arm64.zip
sudo mv belter /usr/local/bin/
belter --help
```

On Linux:

```bash
tar -xzf belter-cli-<version>-linux-x64.tar.gz
sudo mv belter /usr/local/bin/
belter --help
```

To work on the Belter files in a folder:

```bash
belter --root ./my-designs tools
```

## Check a download

The macOS app and the macOS command-line tool are signed with an Apple Developer ID and notarised by Apple. macOS
checks this when you open them.

The Linux files are not signed. Check every file against `SHA256SUMS`:

```bash
shasum -a 256 -c SHA256SUMS --ignore-missing
```

## Licence

Belter is free to use. It is not open source (yet). Read [LICENSE](LICENSE) for the terms.

## Report a problem

Open an [issue](https://github.com/mikills/trybelter/issues).
