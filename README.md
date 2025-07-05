# Aptx4869AC-plugin-live2d

1. Live2D 看板娘，使用jsDelivr CDN加速静态资源
2. 可以直接使用，如需自定义喜欢的模型，请访问另一个仓库：https://github.com/Aptx4869AC



## **🚀 ** 快速使用

### ① 本地预览

使用 VSCode 等前端工具运行 `test.html` 即可

### ② Hexo 博客支持

在Hexo配置文件中添加以下路径即可使用：

```javascript
live2d: 
  base: https://fastly.jsdelivr.net/gh/Aptx4869AC/plugin-live2d@4.0/ /* 版本号可能需要更改 */
  js: https://fastly.jsdelivr.net/gh/Aptx4869AC/plugin-live2d@4.0/js/live2d-autoload.js /* 版本号可能需要更改 */
```



## **⚙️** 拓展

您可以修改配置文件及对应版本号，使用其他资源。比如`@4.0`为我当前最新版本号。



### 配置文件修改

#### **js\live2d-autoload.js**

```javascript
class Live2d {
  #path;
  #config;
  defaultConfig = {
    apiPath: "https://fastly.jsdelivr.net/gh/Aptx4869AC/plugin-live2d@4.0/api/", /* 版本号更改 */
    isTools: true,
    tools: ["hitokoto", "switch-model", "switch-texture", "photo", "info", "quit"],
    version: "1.0.1",
    tipsPath: "live2d-tips.json",
  };
}
```

#### **api\models.json**

```javascript
{
  "models": {
    "1": {
      "name": "加藤惠",
      "path": "https://fastly.jsdelivr.net/gh/Aptx4869AC/plugin-live2d@4.0/myModel/加藤惠live2d/model/katou_01/katou_01.model.json" /* 版本号更改 */
    },
    "2": {
      "name": "雷姆", 
      "path": "https://fastly.jsdelivr.net/gh/Aptx4869AC/plugin-live2d@4.0/myModel/蕾姆live2d/model/rem/rem.json" /* 版本号更改 */
    }
  }
  ..... (其他也如此)
}
```





## 🎨 可用模型
### 1. 加藤惠
![image-20250705180313794](README.assets/image-20250705180313794.png)



### 2. 雷姆
![image-20250705180256312](README.assets/image-20250705180256312.png)









## 🛠️ 工具栏功能
- hitokoto、switch-model 、switch-texture 、photo 、info 、quit 



## License

如果对您有帮助，**请给个Star ⭐**

Copyright :copyright:2025 [Aptx4869AC](https://github.com/Aptx4869AC)

