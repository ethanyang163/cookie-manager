# cookie-manager
一个轻量、简单、易于使用的cookie管理库

![GitHub](https://img.shields.io/github/license/mashape/apistatus.svg) ![PyPI - Status](https://img.shields.io/pypi/status/Django.svg)

cookie-manager为管理cookie提供简易的方法。
- 没有依赖
- 支持AMD，CommonJS，Node modules
- 仅1KB大小
- 兼容所有浏览器

## 安装
使用npm安装
```console
npm install @psyduck4u/cookie-manager
```
下载`cookie-manager.min.js`在你的项目中引入即可。
```html
<script src="cookie-manager.min.js"></script>
```

## 使用
```js
import CookieManager from '@psyduck4u/cookie-manager';
```
或者在引入`cookie-manager.min.js`之后，你就可以使用`CookieManager`对象了。

## 方法

### 创建cookie
```js
  CookieManager.set(name, value, expires, domain, path, secure);
```

- `name (String)` cookie name
- `value (String)` cookie value
- `expires (Optional) (String)` cookie expiration in days
- `domain (Optional) (String)` cookie domain
- `path (Optional) (String)` cookie path
- `name (Optional) (Boolean)` cookie ssl support flag

### 获取cookie
```js
  CookieManager.get(name);
```

- `name (String)` cookie name

### 更新cookie
```js
  CookieManager.update(name, value, expires, domain, path, secure);
```

- `name (String)` cookie name
- `value (String)` cookie value
- `expires (Optional) (String)` cookie expiration in days
- `domain (Optional) (String)` cookie domain
- `path (Optional) (String)` cookie path
- `name (Optional) (Boolean)` cookie ssl support flag

### 删除cookie
```js
  CookieManager.remove(name);
```

- `name (String)` cookie name


### 获取所有cookie
```js
  CookieManager.getAll();
```

### 清除所有cookie
```js
  CookieManager.clear();
```

## 作者与许可
Created and maintained by [Yuxiang Yang](https://github.com/psyduck4you) under [MIT](LICENSE) License


