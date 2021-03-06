## RPostgres 0.1-9 (2017-11-23)

- Improve DBI compliance for `dbBind()` and others, in particular for the `BYTEA` data type, and for 64-bit integer support and transactions (#51, #64, #66, #68, #98, #101).


## RPostgres 0.1-8 (2017-11-09)

- Improve DBI compatibility (#24, #41, #52, #53, #61, #62, #70, #79, #104, #121).
- Define `timegm` for Windows and add missing function (#136).
- The time zone is set by executing `SET TIMEZONE='UTC'` instead of setting an environment variable (#136).


## RPostgres 0.1-7 (2017-11-06)

- All tests pass again.
- Default to `row.names = FALSE`.
- Fix escaping of `NA` values and character data (@jimhester).
- Consistent coding style.
- Fix `dbDataType()` for data frames (#133, @etiennebr).
- Add support for dates and times (#111, @thrasibule).
- `dbWriteTable()` gains `field.types` argument (#45, @robertzk).
- Implement `dbListFields()` (#41, @thrasibule).
- Fix compiler warnings.


## RPostgres 0.1-6 (2017-08-31)

- Fix tests (#126, @thrasibule).
- Avoid redundant quoting of strings (#125).
- Add `PGTypes` (#124, @thrasibule).


## RPostgres 0.1-5 (2017-08-07)

- Update Rcpp registration code.
- `dbConnect()` now accepts arbitrary connection parameters in the `...` argument (#83, @thrasibule).
- Handles NA values by converting them to NULL (#82, @thrasibule).
- Handle string quoting and missing values in strings (#89, @jimhester).
- `PKG_CFLAGS` and `PKG_LIBS` are now being set when using `pg_config` for `includedir` and `libdir` (#119, @usman-r).
- Use `BYTEA` instead of `BLOB` for PostgreSQL 9.5 support.


## RPostgres 0.1-4 (2016-12-29)

- Added `pg_config` support, factored `CFLAGS` and `LIBS` as separate steps (#81, @mmuurr).
- Fix roundtrip of `logical` values (#108, @thrasibule).
- Fix documentation warning (#109, @thrasibule).


## RPostgres 0.1-3 (2016-12-28)

- Ignore various test.


# RPostgres 0.1-2 (2016-06-08)

- Use new `sqlRownamesToColumn()` and `sqlColumnToRownames()` (rstats-db/DBI#91).
- Use container-based builds on Travis.
- Upgrade bundled `libpq` to 9.5.2 for Windows builds.


# RPostgres 0.1-1 (2016-03-24)

- Use DBItest for testing (#56).


RPostgres 0.1 (2016-03-24)
===

- Rcpp rewrite, initial version
