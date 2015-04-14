px2-yass
========

__px2-yass__ は、[Pickles 2](http://pickles2.pxt.jp/) の環境に [YASS](https://github.com/k-yasu/YASS/) モジュールセットを組み込みます。


## Usage - 使い方

Pickles2 をセットアップする。

composer.json に、下記を追加する。

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

`$ composer update` を実行する。

`px-files/config.php` に、下記のように追加する。

```
// config for Plugins.
$conf->plugins = new stdClass;

// config for Pickles2 Desktop Tool.
$conf->plugins->px2dt = new stdClass;
$conf->plugins->px2dt->paths_module_template = [
	"YASS" => "./vendor/tomk79/px2-yass/px2dt_modules/"
];
```

