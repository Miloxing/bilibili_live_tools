# 弹幕发送

## 简介
使用已登录cookies在bilibili直播中发送弹幕的程序

## 使用

1. 从浏览器中提取cookies:

    1. 浏览器中打开一个空白标签页
    2. 按F12开启开发者工具，进入网络面板
    3. 在该标签页中打开 live.bilibili.com 或其他已登录的bilibili网页
    4. 从开发者工具网络面板中找到最顶部的请求，右键选择复制该请求数据头
    5. 将请求数据头中包含cookies的那一行存入和脚本同文件夹的 `bilicookies.txt` 中

2. 选择要发送弹幕的直播间，途径有三种:

    * 修改脚本顶部的ROOM为该直播间ID
    * 将该直播间ID以命令行参数形式直接附上
    * 直接运行脚本后输入直播间ID

3. 在提示符后输入弹幕消息，按回车发送，程序会显示服务器返回的信息，其中code为0且msg为空表示发送成功，<ctrl+c> 退出程序。