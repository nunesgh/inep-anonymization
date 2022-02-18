# inep-anonymization

## ARX version

The `jar` files in `arx/jars/` were compiled from the ARX fork made by @ramongonze (https://github.com/ramongonze/arx), based on commit https://github.com/ramongonze/arx/commit/8a936d3d5607b8f10957c16c1e2781d94b9f2904 and using the command `ant -buildfile build.xml`.

This fork allows for the creation of matrices with up to (2^31-1)^2 cells, instead of the original limit of up to 2^31-1 cells. Due to some GUI errors caused by the new feature, it is necessary to run ARX via CLI. For more information, see https://github.com/arx-deidentifier/arx/pull/299.
