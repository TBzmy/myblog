---
title: Mirrorx
date: 2020-02-26 11:18:28
tags: 前端
---
# Mirror 简介
**mirrorx是将react、redux及react-router的封装，是一个很好用的react框架**
当我们在使用react框架编写代码时，不可避免的使用redux来做状态管理，我们需要调用dispatch方法来dispatch所有的action。我们就需要在创建一个actions目录来编写所有的action type和action creator，并且我们需要使用异步的action时需要middleware来进行处理。在redux中我们就需要相对应的switch来捕捉所有的action type。当我们开发的页面过多时，这对于代码就过于繁杂，会产生过多的类似代码和多个文件。