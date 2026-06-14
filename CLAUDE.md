# KIM ORDER 项目说明

## 项目概述
KIM FROZEN FOOD SDN BHD内部订单管理工具，托管在GitHub Pages。
前端：HTML/CSS/JS单文件，仓库：thohui888-blip/KIMORDER
后端：Google Apps Script独立项目（KIM ORDER），接收POST请求写入Google Sheets。
每天需要更新Sheets ID。

## 车次分组规则
订单按delivery车次分组：A、B、C、D、E、F、G、JW、BP、其他
- 车次字母在客户名称或备注中识别
- NEW = 新客户，需特别标注
- 加货 = 补单追加，合并到同一客户
- 取消 = 删除该项
- 分单 = 同一客户拆成多张单

## 已知边缘案例
（后续补充踩过的坑）

## 重要提醒
- 改动前先给我看diff再提交
- 不要动Google Sheets写入的字段格式