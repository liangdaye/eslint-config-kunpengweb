eslint-config-kunpengweb
===========================

[![npm package](https://img.shields.io/npm/v/eslint-config-kunpengweb.svg?style=flat-square)](https://www.npmjs.com/package/eslint-config-kunpengweb)
[![NPM downloads](http://img.shields.io/npm/dt/eslint-config-kunpengweb.svg?style=flat-square)](https://npmjs.org/package/eslint-config-kunpengweb)

水晶业务团队ESLint共享配置规则

## 安装

```
$ npm install -g eslint eslint-config-kunpengweb
```

## 文档
* [规则解释](RULE.md)

## 使用
一旦`eslint-config-kunpengweb`安装成功，你可以通过[ESLint配置文件]((http://eslint.cn/docs/user-guide/configuring)) 中的字段extends中使用它

```js
{
  "extends": "kunpengweb",
  "rules": {
    // Additional, per-project rules...
  }
}
```

### 配合`eslint:recommended`使用`kunpengweb`
有部分[eslint:recommended](http://eslint.cn/docs/rules/)提到的规则在kunpengweb中没有提到，因此最好配合eslint:recommend一起使用。

只需要同时继承eslint:recommend 和 kunpengweb 即可，确保 kunpengweb 放置在最后。部分eslint:recommend定义的规则有点严格，kunpengweb里面有做定制化的修改。

```js
{
  "extends": ["eslint:recommended",  "kunpengweb"],
  "rules": {
    // Additional, per-project rules...
  }
}
```


## 版本日志

[版本日志](CHANGELOG.md)

## 许可证

Apache-2 © IVWEB
