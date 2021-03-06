# SINGA:PURA (SINGApore: Polyphonic URban Audio)
![](https://img.shields.io/badge/version-v1.0-green) ![License](https://img.shields.io/badge/license-CC%20BY--SA%204.0-brightgreen) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5645825.svg)](https://doi.org/10.5281/zenodo.5645825) 

The SINGA:PURA dataset is a strongly-labelled polyphonic urban sound dataset with spatiotemporal context. The data were collected via a number of recording units deployed across Singapore as a part of a wireless acoustic sensor network. These recordings were made as part of a project to identify and mitigate noise sources in Singapore, but also possess a wider applicability to sound event detection, classification, and localization. The taxonomy we used for the labels in this dataset has been designed to be compatible with other existing datasets for urban sound tagging while also able to capture sound events unique to the Singaporean context. Please refer to our conference paper published in APSIPA 2021 for more details regarding the data collection, annotation, and processing methodologies for the creation of the dataset.

> K. Ooi, K. N. Watcharasupat, S. Peksi, F. A. Karnapi, Z.-T. Ong, D. Chua, H.-W. Leow, L.-L. Kwok, X.-L. Ng, Z.-A. Loh, W.-S. Gan, "A Strongly-Labelled Polyphonic Dataset of Urban Sounds with Spatiotemporal Context," in Proceedings of the 13th Asia Pacific Signal and Information Processing Association Annual Summit and Conference, 2021. [[paper]](https://arxiv.org/abs/2111.02006)

# Accessing via Soundata

🆕 SINGA:PURA is now accessible via [soundata](https://github.com/soundata/soundata)!

## Installation
Requires `soundata v0.1.1` and above.
```
pip install soundata --upgrade
```

## Usage
```python
import soundata

dataset = soundata.initialize('singapura')
dataset.download()  # download the dataset
dataset.validate()  # validate that all the expected files are there

example_clip = dataset.choice_clip()  # choose a random example clip
print(example_clip)  # see the available data
```

## Documentation
https://soundata.readthedocs.io/en/stable/source/soundata.html#module-soundata.datasets.singapura

# Accessing raw dataset

- ✅ [Labelled subset via Zenodo](https://zenodo.org/record/5645825)
- ✅ [Full dataset including unlabelled subset via DR-NTU](https://researchdata.ntu.edu.sg/dataset.xhtml?persistentId=doi:10.21979/N9/Y8UQ6F)

# License
Creative Commons Attribution-ShareAlike 4.0 International.

# How to Cite
```bibtex
@inproceedings{ooi2021singapura,
    author    = "K. Ooi and K. N. Watcharasupat and S. Peksi and F. A. Karnapi and Z.-T. Ong and D. Chua and H.-W. Leow and L.-L. Kwok and X.-L. Ng and Z.-A. Loh and W.-S. Gan",
    title     = "A Strongly-Labelled Polyphonic Dataset of Urban Sounds with Spatiotemporal Context",
    booktitle = "Proceedings of the 13th Asia Pacific Signal and Information Processing Association Annual Summit and Conference",
    location  = "Tokyo, Japan"
    year      = 2021
}
```
