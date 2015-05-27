# Twig Assetic Fixer

如果你正好在使用 [Twig](http://twig.sensiolabs.org/) + [Assetic](https://github.com/kriswallsmith/assetic) 並且遇到 debug = true 或 combine = false 時，檔案依然合併為一個的問題，那麼此修正檔或許可以幫助你。

### 安裝

```
"wake/Twig-Assetic-Fixer": "*"
```

### 使用

參考 [Assetic#Twig](https://github.com/kriswallsmith/assetic#twig)，最下方有提到 `These assets need to be written to the web directory so these URLs don't return 404 errors.`，請將原本 `TwigFormulaLoader` 的部份更改為 `TwigFormulaFixerLoader`。

```
use TwigAsseticFixer\TwigFormulaFixerLoader;
```

```
$am->setLoader('twig', new TwigFormulaFixerLoader($twig));
```

### 回報

有任何疑問或需要協助的歡迎開 issue。
