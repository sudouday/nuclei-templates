# Nuclei Hidden File Fuzzing Template

A custom **Nuclei** template designed to discover hidden or sensitive files by fuzzing common file and directory names on a target website.

## Features

* 🔍 Fuzzes for common hidden and sensitive files.
* ⚡ Fast scanning using the Nuclei engine.
* 🛠️ Easily customizable—add your own file names or paths to improve coverage.
* 🎯 Useful during reconnaissance and security assessments.

## Requirements

* [Nuclei](https://github.com/projectdiscovery/nuclei)
* A target domain or subdomain

## Usage

Run the template against a target using the `-u` (URL) and `-t` (template) options:

```bash
nuclei -u https://www.airtel.com -t /root/nuclei-templates/exposures/files/hiddenfiles.yaml
```

### Example

```bash
nuclei -u https://example.com -t /path/to/hiddenfiles.yaml
```

## How It Works

The template fuzzes a list of common hidden or sensitive file names against the specified target and reports any files that are accessible. This can help identify:

* Backup files
* Configuration files
* Temporary files
* Hidden resources
* Other unintentionally exposed files

## Customization

You can improve detection by adding your own file names or paths to the wordlist used in the template. The more relevant entries you include, the better your chances of discovering exposed resources.

## Disclaimer

This template is intended **only for authorized security testing and educational purposes**. Always obtain proper permission before scanning any target.

