# data-default-instances-text

[![Hackage](http://img.shields.io/hackage/v/data-default-instances-text.svg)][data-default-instances-text]
[![Hackage Dependencies](https://img.shields.io/hackage-deps/v/data-default-instances-text.svg)](http://packdeps.haskellers.com/reverse/data-default-instances-text)
[![Haskell Programming Language](https://img.shields.io/badge/language-Haskell-blue.svg)][Haskell.org]
[![BSD3 License](http://img.shields.io/badge/license-BSD3-brightgreen.svg)][tl;dr Legal: BSD3]

[![Build](https://travis-ci.org/trskop/data-default-extra.svg)](https://travis-ci.org/trskop/data-default-extra)


# Description

`Default` instances for types defined in [text][] package:

```Haskell
instance Default Strict.Text where
    def = Strict.Text.empty

instance Default Lazy.Text where
    def = Lazy.Text.empty

-- For text >=0.8
instance Default Builder where
    def = mempty
```

Following instances are provided only for [text][] >=0.8, since that
it the version that introduced `Builder`:

```Haskell
instance Default Builder where
    def = mempty
```

This package is intended to be used in conjunction with [data-default][]
package or directly with [data-default-class][] package.


## License

The BSD 3-Clause License, see [LICENSE][] file for details.


## Contributions

Contributions, pull requests and bug reports are welcome! Please don't be
afraid to contact author using GitHub or by e-mail.


[data-default]:
  https://hackage.haskell.org/package/data-default
  "Package data-default on Hackage"
[data-default-class]:
  https://hackage.haskell.org/package/data-default-class
  "Package data-default-class on Hackage"
[data-default-instances-text]:
  https://hackage.haskell.org/package/data-default-instances-text
  "Package data-default-instances-text on Hackage"
[Haskell.org]:
  http://www.haskell.org
  "The Haskell Programming Language"
[LICENSE]:
  https://github.com/trskop/data-default-extra/blob/master/instances-text/LICENSE
  "License of data-default-instances-text package."
[text]:
  https://hackage.haskell.org/package/text
  "Package text on Hackage"
[tl;dr Legal: BSD3]:
  https://tldrlegal.com/license/bsd-3-clause-license-%28revised%29
  "BSD 3-Clause License (Revised)"
