px2-yass
========

__px2-yass__ は、[Pickles 2](http://pickles2.pxt.jp/) の環境に [YASS](https://github.com/k-yasu/YASS/) モジュールセットを組み込みます。


## Usage - 使い方

### 1. Pickles2 をセットアップ

### 2. composer.json に追記

```
{
    "repositories": [
        {
            "type": "git",
            "url": "https://github.com/tomk79/px2-yass.git"
        }
    ],
    "require": {
        "tomk79/px2-yass": "dev-master"
    }
}
```

### 3. composer を更新

```
$ composer update
```

### 4. px-files/config.php に追加

```
// config for Pickles2 Desktop Tool.
@$conf->plugins->px2dt->paths_module_template["YASS"] = "./vendor/tomk79/px2-yass/modules/";
```

