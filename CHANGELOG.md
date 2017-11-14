# 0.2.1

## Api Breakage

* Changed BTree containers in analysis/use_def to Hash containers.
* Moved store/load methods from `domain::Memory` to `domain::Domain`
* Remove `endian()` method from `Translator` trait.

## Fixes

* Removed unused regex and lazy_static crates.
* Removed `Display + Serialize` trait requirements for `domain::Value`
* Relax trait requirements for `domain::Expression`
* Fixed a bug in `KSetDomain::load`

## Additions

* Add `stack_pointer` function `types::Architecture`
* Add `locations`, and `blocks_mut` functions to `il::Function`
* Add an `into_` method for `domain::Expression` to help translate expressions between domains.
* Add `symbolize`, `remove_variable`, and `memory_mut` functions to `domain::State`
* Add support for `Mipsel`, as it's only a minor change from Mips.