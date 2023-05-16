# Generale missiven (RGP volumes)

This repo contains the sections of the published volumes of the Generale missiven of the VOC (<https://resources.huygens.knaw.nl/retroboeken/generalemissiven/>) with transcriptions of the original letters. All introductions, footnotes, indices and summaries (in modern Dutch) are omitted. It uses the Text Fabric version of the Generale missiven volumes developed by Dirk Roorda in the context of CLARIAH: <https://github.com/CLARIAH/wp6-missieven/> 

## Use Text Fabric to extract transcriptions of original letters from each volume

First, install Text Fabric:

```bash
pip3 install text-fabric
```

Then download the Generale missiven:

```bash
text-fabric clariah/wp6-missieven
```

Use Python to extract the sections containing transcriptions of original letters: <(https://github.com/globalise-huygens/globalise-generale-missiven-rgp/blob/main/tf.ipynb>. Copy the output to a txt file.

## Split txt files and sort them into folders

Use Python to split the txt files that contain all original transcriptions of a volume into files separate files for each page. Use the references to volume, page and line on each line of the large txt file to name the newly created files and move them to a subdirectory. Also, remove the leading whitespace on each line and any blank lines. See <https://github.com/globalise-huygens/globalise-generale-missiven-rgp/blob/main/split_large_txt_file_into_smaller.ipynb> for the method used.

