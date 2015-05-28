# Twig Assetic Fixer

Twig-Assetic-Fixer try to fix the issue: `debug = true`, `combine = false` options not work, the asset files always combined when using [Twig](http://twig.sensiolabs.org/) with [Assetic](https://github.com/kriswallsmith/assetic).


### Install

Install by Composer

```
"require": {
  "wake/Twig-Assetic-Fixer": "*"
}
```


### Use

Check last section of [Assetic#Twig](https://github.com/kriswallsmith/assetic#twig), replace 

``` php
use Assetic\Extension\Twig\TwigFormulaLoader;
```

with

``` php
use TwigAsseticFixer\TwigFormulaLoader;
```

----

# Twig Assetic Fixer

如果你正好在使用 [Twig](http://twig.sensiolabs.org/) + [Assetic](https://github.com/kriswallsmith/assetic) 並且遇到 debug = true 或 combine = false 時，檔案依然合併為一個的問題，那麼此修正檔或許可以幫助你。


### 安裝

透過 Composer 安裝

```
"require": {
  "wake/Twig-Assetic-Fixer": "*"
}
```

### 使用

參考 [Assetic#Twig](https://github.com/kriswallsmith/assetic#twig)，最下方有提到 `These assets need to be written to the web directory so these URLs don't return 404 errors.`，請將原本

``` php
use Assetic\Extension\Twig\TwigFormulaLoader;
```

改換成

``` php
use TwigAsseticFixer\TwigFormulaLoader;
```

### 回報

有任何疑問或需要協助的歡迎開 issue :smirk:



