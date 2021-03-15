---
title: ECharts
date: 2020-02-26 11:18:28
tags: 前端
---
# ECharts 初探
**简介**
EChart是使用JS实现的开源可视化库，涵盖各行业的图标，兼容绝大部分的浏览器
> 简单实例
```html
<head>
    <meta charset="utf-8">
    <title>第一个 ECharts 实例</title>
    <!-- 引入 echarts.js -->
    <script src="https://cdn.staticfile.org/echarts/4.3.0/echarts.min.js"></script>
</head>
<body>
    <!-- 为ECharts准备一个具备大小（宽高）的Dom -->
    <div id="main" style="width: 600px;height:400px;"></div>
    <script type="text/javascript">
        // 基于准备好的dom，初始化echarts实例
        var myChart = echarts.init(document.getElementById('main'));
 
        // 指定图表的配置项和数据
        var option = {
            title: {
                text: '第一个 ECharts 实例'
            },
            tooltip: {},
            legend: {
                data:['销量']
            },
            xAxis: {
                data: ["衬衫","羊毛衫","雪纺衫","裤子","高跟鞋","袜子"]
            },
            yAxis: {},
            series: [{
                name: '销量',
                type: 'bar',
                data: [5, 20, 36, 10, 10, 20]
            }]
        };
 
        // 使用刚指定的配置项和数据显示图表。
        myChart.setOption(option);
    </script>
</body>
```
> 运行结果
<!-- ![运行结果](1.jpg) -->
