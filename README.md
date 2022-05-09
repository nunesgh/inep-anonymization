# INEP [^inep] (syntactic) Anonymization

Code and attributes hierarchies used for the anonymization process of INEP datasets using [ARX Deidentifier](https://github.com/arx-deidentifier/arx) tool.

DOI: [10.5281/zenodo.6533684](https://doi.org/10.5281/zenodo.6533684).

The resulting datasets were used for vulnerability assessment using the [BVM library](https://github.com/nunesgh/bvm-library) ([10.5281/zenodo.6533704](https://doi.org/10.5281/zenodo.6533704)). The assessment results were published in: Mário S. Alvim, Natasha Fernandes, Annabelle McIver, Carroll Morgan, Gabriel H. Nunes - _Flexible and scalable privacy assessment for very large datasets, with an application to official governmental microdata_ (2022, [10.48550/arXiv.2204.13734](https://doi.org/10.48550/arXiv.2204.13734)).

We randomly selected only one record for each student with a same unique pseudonymization code (`ID_ALUNO`) in each dataset. The enrollment code (`ID_MATRICULA`) for each selected record is available in [10.5281/zenodo.6533675](https://doi.org/10.5281/zenodo.6533675) ([gitlab.com/nunesgh/inep-enrollment-codes](https://gitlab.com/nunesgh/inep-enrollment-codes)).

## ARX version

The `jar` files in `arx/jars/` were compiled from the [ARX fork](https://github.com/ramongonze/arx) made by [@ramongonze](https://github.com/ramongonze), based on commit [8a936d3](https://github.com/ramongonze/arx/commit/8a936d3d5607b8f10957c16c1e2781d94b9f2904) and using the command `ant -buildfile build.xml`.

This fork allows for the creation of matrices with up to (2^31-1)^2 cells, instead of the original limit of up to 2^31-1 cells. Due to some GUI errors caused by the new feature, it is necessary to run ARX via CLI. For more information, see [this issue](https://github.com/arx-deidentifier/arx/pull/299).

## License

[The Unlicense](https://choosealicense.com/licenses/unlicense/).

[^inep]:
    The [Anísio Teixeira National Institute of Educational Studies and Research](https://www.gov.br/INEP).

