---
title: dfr all-false
categories: |
  dataframe
version: 0.76.0
dataframe: |
  Returns true if all values are false
usage: |
  Returns true if all values are false
---

# <code>{{ $frontmatter.title }}</code> for dataframe

<div class='command-title'>{{ $frontmatter.dataframe }}</div>

## Signature

```> dfr all-false ```

## Examples

Returns true if all values are false
```shell
> [false false false] | dfr into-df | dfr all-false
```

Checks the result from a comparison
```shell
> let s = ([5 6 2 10] | dfr into-df);
    let res = ($s > 9);
    $res | dfr all-false
```