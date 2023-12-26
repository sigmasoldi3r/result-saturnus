# Result (Saturnus)

A simple library inspired by Rust's std result type.

```rs
use { Ok, Err } in result;

fn something_that_might_fail(a, b) {
    if b == 0 {
        return Err("Divide by 0!");
    } else {
        return Ok(a / b);
    }
}

let ok_value = something_that_might_fail(1, 2)->unwrap();
// ok_value == 0.5
```

## Installation

Just add this line to the Janus file, under `[dependencies]`:

```toml
result = { git = "https://github.com/sigmasoldi3r/result-saturnus" }
```
