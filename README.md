# Test Library for SCPL

Minimal assertions for validating SCPL programs and libraries.

## Exported Functions

- `assert-true value label`
- `assert-false value label`
- `assert-eq actual expected label`
- `assert-type value expected label`
- `assert-neq actual expected label`
- `assert-nil value label`
- `assert-error value label`
- `assert-ok value label`
- `test-report passed total`

## Usage

```scpl
import test
Initialize-console

assert-true: true 'boolean true works'
assert-false: false 'boolean false works'
assert-eq: (+ 2 2) 4 'math works'
assert-type: (dict 'name' 'SCPL') 'dict' 'dict type works'
assert-ok: (ok 42) 'ok result works'
assert-error: (error 'boom') 'error result works'
test-report: 6 6

Close-console
```
