# Illuminate Light Collections

This package provides Illuminate Collections minus hundreds of contracts from
`Illuminate\Contracts` that are not used by this library.

This library can be used for external libraries or projects that don't depend on
Laravel framework. 

## Install

```shell
composer req bafs/illuminate-light-collections
```

## Why?

Illuminate collections is a handy library to work will collections, but it requires
`illuminate/contracts` which provides hundreds of contracts from the Illuminate framework
and that are not useful when working outside the Laravel ecosystem. Only 3 contracts are
used by Collections (`Arrayable`, `CanBeEscapedWhenCastToString`, `Jsonable`).

## I don't like monkey patching, can I remove it too?

Yes, it's also possible to disable the monkey patching from the
[Macroable](https://github.com/illuminate/macroable) library (`illuminate/macroable`).
To do so, use the [Demacroable](https://github.com/BafS/Demacroable) package
(`bafs/illuminate-demacroable`) in your project (it will replace the Macroable trait with an empty one).
