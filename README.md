# Morphological Analyzer for Shipibo-Konibo

Shipibo-Konibo (SK) is a native language mainly spoken in the Amazonian regions of Pery by nearly 30,000 people.
This repository contains a morphological analyzer for this language.
Tha analyzer is a FST that produces all posible segmentations and tagging sequences in a word-by-word fashion.


## Requirements
You will only need [foma](https://fomafst.github.io/)

## Usage
First, compile the FST from *foma_files* directory

```bash
foma -f analyzer.foma
```

The analyzer reads and writes to stdin/stdout.
The text must be in one-word-per-line format.

```bash
cat sample-input.txt | flookup morph_shk.fst
```


## Cite us

If you use this tool, please consider citing the following papers


