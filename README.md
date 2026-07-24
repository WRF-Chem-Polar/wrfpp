The python package wrfpp (think "WRF post-processing") facilitates the analysis of WRF and WRF-Chem outputs.

It was originally part of our [WRF-infra](https://github.com/WRF-Chem-Polar/WRF-infra) repository but is now a stand-alone Python package.

It works with native WRF and WRF-Chem outputs as well as [WRF-Chem-Polar](https://github.com/WRF-Chem-Polar/WRF-Chem-Polar) outputs.

# Installing wrfpp

> [!TIP]
> We strongly encourage you to work within some kind of isolated Python environment (eg. [venv](https://docs.python.org/3/library/venv.html) or [conda](https://docs.conda.io/en/latest/))

You can install `wrfpp` with `pip`. It is recommended to install a tagged version (eg. "v1.0"):

```sh
pip install wrfpp[all]@git+https://github.com/WRF-Chem-Polar/wrfpp.git@v1.0
```

To install the latest development version, simply omit the tag:

```sh
pip install wrfpp[all]@git+https://github.com/WRF-Chem-Polar/wrfpp.git
```

You can choose not to install optional dependencies by omitting `[all]` in the commands above. Some features of `wrfpp` will not work in this case.

# Versioning

For reproducible computing, please only use commits tagged with a version number (eg. "v2.3"). These uniquely and unequivocally define specific versions of wrfpp. This is **not** true for any version number that has the ".dev0" suffix (eg "v2.3.dev0").

# Authorship

## Institutions

The wrpp package is developed at the [Laboratoire Atmosphères et Observations Spatiales](https://latmos.ipsl.fr/) (LATMOS, UMR 8190) and the [Institut des Géosciences de l'Environnement](https://www.ige-grenoble.fr/) (IGE, UMR 5001), both located in France.

## Individual contributing authors

Below are listed (in alphabetical order of last names) all the individual authors that contributed to wrfpp. Contributions can include small and large developments and/or code reviews. Use Git and Github for more detailed information about authorship (see our [WRF-infra](https://github.com/WRF-Chem-Polar/WRF-infra) repository for early versions of wrfpp).

 - Lucas Bastien
 - Lucas Giboni
 - Erfan Jahangir
 - Rémy Lapere
 - Louis Marelle
 - Ruth Price
 - Jennie Thomas
