# Ajax

## XMLHttpRequest

> - [XMLHttpRequest API](https://developer.mozilla.org/en-US/docs/Web/API/XMLHttpRequest_API)
> - [XMLHttpRequest](https://developer.mozilla.org/en-US/docs/Web/API/XMLHttpRequest)

- **原生 JavaScript API**：XHR 是浏览器原生提供的 API，用于进行异步通信。
- **回调风格**：XHR 使用回调函数的方式来处理异步操作，通常需要设置 `onreadystatechange` 事件回调。
- **老式，不够现代**：相对较老，不支持 Promise 风格的编程，对于复杂的异步操作可能显得不够现代化。

### 跨域请求携带 Cookie

> [withCredentials 属性 - MDN](https://developer.mozilla.org/zh-CN/docs/Web/API/XMLHttpRequest/withCredentials)

```js
const xhr = new XMLHttpRequest()
xhr.open("GET", "http://example.com/", true)
xhr.withCredentials = true
xhr.send(null)
```

## Fetch

> [Fetch API](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API)
> [Fetch()](https://developer.mozilla.org/en-US/docs/Web/API/fetch)

- **现代 API**：Fetch 是现代的 Web API，提供了更简单和强大的方式来进行网络请求。
- **Promise 风格**：Fetch 基于 Promise，使异步代码更易管理，支持流式操作。
- **内置 JSON 支持**：Fetch 内置支持 JSON 解析，响应对象是一个 Response 对象，可以使用内置方法进行处理。
- **不支持老浏览器**：不支持 Internet Explorer 11 及更早版本的浏览器，需要使用 polyfill 进行兼容性处理。

## jQuery.ajax()

> [jQuery.ajax()](https://api.jquery.com/jQuery.ajax/)

jQuery Ajax 是 jQuery 库的一部分，封装了底层的 `XMLHttpRequest`，提供了更高级的接口，隐藏了许多底层细节，以简化异步请求的处理。

## Axios

> [Axios](https://www.axios-http.cn/docs/intro)

Axios 是一个基于 promise 网络请求库，作用于node.js 和浏览器中。 它是 isomorphic 的(即同一套代码可以运行在浏览器和node.js中)。在服务端它使用原生 node.js http 模块, 而在客户端 (浏览端) 则使用 XMLHttpRequests。

## API 搜集

### 国内 API

- [聚合数据](https://www.juhe.cn/)
- [蜻蜓 FM](https://open.qingting.fm/)
- [七牛云](https://developer.qiniu.com/)

### 国外 API

- https://github.com/public-apis/public-apis
- https://github.com/fangzesheng/free-api
- [GitHub API](https://developer.github.com/v3/)：GitHub API。
- https://designer.mocky.io/
- https://reqres.in/
- https://jsonplaceholder.typicode.com/
- https://worldtimeapi.org/
- https://timeapi.io/
- [OpenWeatherMap](https://openweathermap.org/api)：天气数据 API。
- [Unsplash](https://unsplash.com/developers)：图片 API。

### 其他

[跨域](https://cors-anywhere.herokuapp.com/corsdemo)
