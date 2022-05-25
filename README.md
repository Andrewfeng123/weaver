# Weaver

## SMT solvers

For Windows users:

* Download Yices and place the executable ``yices-smt2`` in this directory
* Download CVC4 and place the executable ``cvc4`` in this directory (rename ``cvc4-1.x...`` to ``cvc4``) 
* Do the same for ``mathsat`` (plus all the dll's in the ``bin`` directory of ``mathsat``)

## Build

```
git clone https://github.com/weaver-verifier/weaver
cd weaver
cabal new-build weaver
```

## Example

```
cabal new-run weaver -- examples/parallel/parallel-sum-1.wvr -m partition-progress -b rr
```
