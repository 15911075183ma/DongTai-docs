---
sidebar_position: 1
---

# 项目配置

项目配置在上方菜单栏的左边第一个，功能是展示已创建的项目，其子功能如下：

## 新建项目

![Image](../_resource/operation/application/zh_application_new.png)

* 基本设置：项目名称、扫描策略

  * 项目名称和扫描策略是必填选项。

  * 关联 Agent 如果不填写该项目会与和项目名称一致的 Agent 自动绑定。

  * 在 Agent 安装的时候也能设定参数，如：`-Dproject.create=true`，安装后会自动将项目建立好。

  :::info 高级配置

  点选高级设置

  ![Image](../_resource/operation/application/zh_application_new_advanced.png)

  * 主动验证 : 用于验证存在污点调用链的漏洞是否真实有效。（测试功能）

  * 关联 Agent : 手动绑定 Agent。

  * 版本名称 : 为项目设定版本号。

  * 版本描述 : 描述项目版本号。

  * 项目地址 : 配置项目的外部访问地址，API 导航扫描用，仅限：Spring Boot 框架。（测试功能）

  * 访问凭证 : 配置项目的访问凭证，API 导航扫描用，仅限：Spring Boot 框架。（测试功能）

  ::: 
  

## 项目列表

![Image](../_resource/operation/application/zh_application_list.png)

* 展示已创建的项目列表。

## 管理项目

* 编辑项目详情。

* 删除项目。

## 搜索项目

* 搜索项目在项目配置页面右上方，可根据项目名称搜索项目。


## 项目详情

展示项目的详细信息，其子功能如下：

### 项目概述

![Image](../_resource/operation/application/zh_application_detail.png)

* 漏洞分布：漏洞等级直方图，统计漏洞等级和对应数量。
* 类型分布：漏洞类型饼图，统计漏洞类型和对应数量。
* 风险趋势：发现漏洞时间与数量关系折线图，统计漏洞数量和发现时间趋势。


### 项目漏洞

![Image](../_resource/operation/application/zh_application_vul.png)

* 展示项目下所有漏洞的详细信息。

* 漏洞排序可以根据`漏洞类型`、`漏洞等级`、`URL`、`最新上报时间`、`首次上报时间` 五个条件生序或降序排序。

* 过滤器根据`漏洞类型`、`等级`、`语言`进行过滤。

* 漏洞验证对已检测到漏洞进行验证，此功能需要探针存活。

### 项目组件

![Image](../_resource/operation/application/zh_application_component.png)

* 展示项目下所有组件信息。

* 组件排序可根据`风险等级`、`包名`、`版本`、`语言`、`风险数量`五个条件排序；

* 过滤器根据`漏洞等级`、`语言`进行过滤。

### API 导航

![Image](../_resource/operation/application/zh_application_api.png)

* 展示项目下所有所有 API 接口的信息。

* 过滤器可以根据请求方法、覆盖状态进行过滤。

* 搜索根据 API 地址进行搜索。

### 报告导出

![Image](../_resource/operation/application/zh_application_reportbar.png)

* 组件报告：导出 `csv` 档案

* 漏洞报告：导出 `docx`、`pdf`、`xlsx` 档案
