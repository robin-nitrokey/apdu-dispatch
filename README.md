# Tests

For the tests to run locally for ApduDispatch, you need to enable std for logs.

```
cargo test --features std,log-all --target $(rustc -Vv | awk 'NR==5{print $2}')
```
