# echarts

- 两个版本：echarts(平面)、GL(3d)

- 用法：_写配置_

## 个性化图表的样式

- 数据图形样式的设置层级：全局、系列、数据

## 颜色主题

- 在 [主题编辑器](http://echarts.baidu.com/theme-builder/) 构建主题，保存为 JSON 文件

- 获取 JSON

- 注册主题

- 初始化 echarts 实例和加载主题

```javascript
    $.getJSON("../theme/chalk.json", themeJSON => {
    // 获取主题 JSON
    echarts.registerTheme("chalk", themeJSON); // 注册
    resolve(echarts.init(oBox, "chalk")); // 初始化实例和加载主题
    });
```
