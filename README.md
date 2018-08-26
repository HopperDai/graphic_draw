# 平面绘图

- canvas 位图，放大会失真；不储存图形信息，没法修改，没有事件；性能高

- SVG/VML 矢量图，放大不失真；存储图形信息，便于修改、事件；性能一般

- 库

  - Raphael

  - [echarts](http://echarts.baidu.com/) 百度

  - [d3.js](https://d3js.org/) 阿里

    - 下载

      - 从官网下载

      - `bower i d3`

    - 使用 d3 主要操作两件事

      - 计算

      - 生成

  ## echarts

  - 两个版本：echarts(平面)、GL(3d)

  - 基础用法：

    - 通过 `echarts` 初始化表格

    - 定义表格的 **option**

    - 设置 `option`

    ```javascript
    const chart = echarts.init(容器元素);

    let option = {
      // 详细配置需查看官网
      title, // 标题
      xAxis, // 柱状图
      yAxis, // 柱状图
      series: [
        // 数据
        {
          name: "该系列数据的名字",
          type: "bar/pie/radar",
          data: [{ name: "该项数据的名字", value: "数据" }]
        }
      ]
    };

    chart.setOption(option);
    ```

  - 用法：_写配置_
