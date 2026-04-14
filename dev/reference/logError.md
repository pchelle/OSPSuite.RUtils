# logError

Log error with time stamp

## Usage

``` r
logError(msg)
```

## Arguments

- msg:

  Character values of message to log that leverages `cli` formatting.

## Examples

``` r
# Log error
logError(cliFormat("This is an {.strong error} message"))
#> ✖ Error [14/04/2026 - 12:57:49]:  This is an error message
#> 

# Log error with indications
logError(cliFormat(
  "This is an {.strong error} message",
  "Check these {.val values} or this {.fn function}"
))
#> ✖ Error [14/04/2026 - 12:57:49]:  This is an error message
#> → Check these "values" or this `function()`
#> 
```
