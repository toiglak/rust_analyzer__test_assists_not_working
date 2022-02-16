# rust_analyzer bug report: `test_assists_not_working`

This repository shows minimum reproducible example of test assists in rust analyzer breaking.

As far as I am concerned, this bug is related to subcrate being named `core` - possibly overlapping with `std` name?

## Temporary fix

Test assists work again if we rename culprit package from `core` to something else.
