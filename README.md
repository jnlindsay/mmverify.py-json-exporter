# mmverify.py-json-exporter

This is a fork of [David Wheeler's Python Metamath verifier](https://github.com/david-a-wheeler/mmverify.py).

Usage:

```
python3 mmverify.py set.mm --json-export set.json  
```

To export only one proof-step type (for example, only turnstile steps) while keeping original step numbers, use:

```
python3 mmverify.py set.mm --json-export set.json --only-type '|-'
```

To export only a single theorem, say `prmunb`, use:

```
python3 mmverify.py set.mm --json-export prmunb.json --begin-label prmunb --stop-label prminf
```

where `primnf` is the theorem directly after `prmunb` in `set.mm`.
