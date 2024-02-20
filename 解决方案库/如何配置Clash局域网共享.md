# 如何配置Clash局域网共享

| Author     | Date      |
| ---------- | --------- |
| Jeronasand | 2024/2/21 |

[TOC]

## 前提条件

- 已经可以上外网
- 已经安装好clash （文末有clash安装包链接）

## 打开clash

![image-20240221025649747](https://jeronasand.oss-cn-guangzhou.aliyuncs.com//TyporaImages/image-20240221025649747.png)

## 启用 System Proxy 和 Allow LAN 记住静态端口7890

![image-20240221025850809](https://jeronasand.oss-cn-guangzhou.aliyuncs.com//TyporaImages/image-20240221025850809.png)

## 打开 控制面板 > 系统和安全 > Windows Defender 防火墙 > 高级设置 

![image-20240221030148856](https://jeronasand.oss-cn-guangzhou.aliyuncs.com//TyporaImages/image-20240221030148856.png)

## 点击 出站规则 > 新建规则

![image-20240221030252202](https://jeronasand.oss-cn-guangzhou.aliyuncs.com//TyporaImages/image-20240221030252202.png)

## 按照表格内容填写

![image-20240221030340729](https://jeronasand.oss-cn-guangzhou.aliyuncs.com//TyporaImages/image-20240221030340729.png)

| 步骤名称   | 填写参数               |
| ---------- | ---------------------- |
| 规则类型   | 端口                   |
| 协议和端口 | TCP 特定端口 7890      |
| 操作       | 允许连接               |
| 配置文件   | 全选                   |
| 名称       | clash7890 (可以自定义) |

![image-20240221030725586](https://jeronasand.oss-cn-guangzhou.aliyuncs.com//TyporaImages/image-20240221030725586.png)

## 可以看到已经有了

![image-20240221030757820](https://jeronasand.oss-cn-guangzhou.aliyuncs.com//TyporaImages/image-20240221030757820.png)

## 如果尝试还是不行，就把入站规则也重复一下出站规则的步骤即可

## clash 下载链接 

> 链接：https://pan.baidu.com/s/1NJw_NhldvDIYjepbFTCbng?pwd=0001 
> 提取码：0001 
> --来自百度网盘超级会员V3的分享