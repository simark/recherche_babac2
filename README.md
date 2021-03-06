[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)

# Recherche Babac2

A Python3 module to search the Cycle Babac catalogue and return description, price and availability.

## Installation

1. Clone the repository

```bash
git clone https://github.com/normcyr/recherche_babac2
```

2. Create a Python virtual environment using `virtualenv`

```bash
cd recherche_babac2
virtualenv -p python3 venv
source venv/bin/activate
```

3. Install the module

```bash
python setup.py install
```

## Setup the configuration file

```bash
cp config.yml.example config.yml
```

Then edit the `config.yml` file (*eg* `nano config.yml`) and change the value of the `username` and `password` variables to the proper credentials to log in to the Cycle Babac website.

## Perform a search

Launch the search with the following command:

```bash
recherche_babac2 search text
```

For example:

```bash
recherche_babac2 training wheels
```

or, using a catalogue number:

```bash
recherche_babac2 22-150
```
