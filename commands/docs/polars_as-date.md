---
title: polars as-date
categories: |
  dataframe
version: 0.94.0
dataframe: |
  Converts string to date.
usage: |
  Converts string to date.
feature: default
---
<!-- This file is automatically generated. Please edit the command in https://github.com/nushell/nushell instead. -->

# `polars as-date` for [dataframe](/commands/categories/dataframe.md)

<div class='command-title'>Converts string to date.</div>

## Signature

```> polars as-date {flags} (format)```

## Flags

 -  `--not-exact, -n`: the format string may be contained in the date (e.g. foo-2021-01-01-bar could match 2021-01-01)

## Parameters

 -  `format`: formatting date string


## Input/output types:

| input | output |
| ----- | ------ |
| any   | any    |

## Examples

Converts string to date
```nu
> ["2021-12-30" "2021-12-31"] | polars into-df | polars as-date "%Y-%m-%d"

```

## Notes
Format example:
        "%Y-%m-%d"    => 2021-12-31
        "%d-%m-%Y"    => 31-12-2021
        "%Y%m%d"      => 2021319 (2021-03-19)