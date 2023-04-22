# DuckDB Db2 Scanner

The `db2_scanner` extension allows `DuckDB` to directly read data from a running `Db2` instance

## Test

```sh
make test
```

## Building & Loading the Extension

To build, type 
```
make
```

To run, run the bundled `duckdb` shell:
```
 ./build/release/duckdb -unsigned  # allow unsigned extensions
```

Then, load the `Db2` extension like so:
```SQL
LOAD 'build/release/extension/db2_scanner/db2_scanner.duckdb_extension';
```
