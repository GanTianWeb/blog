# HTTP 相关博客
### 博客题：请写一篇博客介绍 HTTP，主要内容有
1. HTTP 请求包括哪些部分，如何用Chrome开发者工具查看 HTTP 请求内容
2. HTTP 响应包括哪些部分，如何用Chrome开发者工具查看 HTTP 响应内容
3. 如何使用 curl 命令

### 答:
1. HTTP 请求包括 
1 GET / HTTP/1.1 (动词路径协议/版本) <br />
2 Host: xiedaimala.com (Key1: value1) <br />
2 User-Agent:  Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/76.0.3809.132 Safari/537.36
Sec-Fetch-Mode: navigate (Key2: value2) <br />
2 Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3
Sec-Fetch-Site: none (Key3: value3) <br />
3 <br />
4 要上传的数据 <br />

2. HTTP 响应包括 <br />
1 协议/版本号,状态码,状态解释 <br />
2 Key1: value1<br />
2 Key2: value2
2 Content-Length: 17931 <br />
2 Content-Type: text/html <br />
3<br />
4 要下载的内容 <br />

3. 如何使用 curl 命令
1 curl -s -v -H "Frank: xxx" -- "https://www.baidu.com" (-H "Frank: xxx" 可换成其他的"Key：value") <br />
2 curl -X POST -s -v -H "Frank: xxx" -- "https://www.baidu.com" (使用POST上传) <br />
3 curl -X POST -d "1234567890" -s -v -H "Frank: xxx" -- "https://www.baidu.com" (使用POST上传的值为1234567890) <br />
4 了解更多[Linux](https://man.linuxde.net// "Linux") <br />

4. 如何使用Chrome开发者工具查看 HTTP 请求or响应内容
1 打开Chrome，右键检查 <br />
2 打开 Network <br />
3 输入网址 <br />
4 选中第一个响应 <br />
5 查看 Response Headers or Requset Headers，点击「view source」 <br />
6 你会看到响应的前两部分 <br />
7 查看 Response 或者 Preview，你会看到响应的第 4 部分 <br />
