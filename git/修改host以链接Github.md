#修改host以链接Github

>步骤
- tap1 打开host文件,将下方`host`的代码粘到里面
  - host文件位于`C:\Windows\System32\drivers\etc\host`
  - 使用记事本打开
  - 粘入代码后保存
- 刷新网络缓存
  - 打开`cmd`(管理员)
  - 运行 `ipconfig /flushdns`

>常见报错
- host 文件在保存时`报错`或者显示`另存为`   
    打开host属性,选择`安全`选项卡,单击`编辑`按钮,选择要修改权限的用户(一般为当前用户),对`完全控制`打钩,然后保存;再执行tap1

>附件
##host
```
199.232.69.194 github.global.ssl.fastly.net
140.82.113.3 github.com
140.82.112.4 www.github.com
185.199.108.153 assets-cdn.github.com
185.199.109.153 assets-cdn.github.com
185.199.110.153 assets-cdn.github.com
185.199.111.153 assets-cdn.github.com
185.199.108.153 documentcloud.github.com
185.199.109.153 documentcloud.github.com
185.199.110.153 documentcloud.github.com
185.199.111.153 documentcloud.github.com
140.82.114.3 gist.github.com
185.199.108.153 help.github.com
185.199.109.153 help.github.com
185.199.110.153 help.github.com
185.199.111.153 help.github.com
140.82.112.9 nodeload.github.com
199.232.68.133 raw.github.com
140.82.112.18 status.github.com
140.82.113.18 training.github.com
199.232.68.133 raw.githubusercontent.com
199.232.68.133 user-images.githubusercontent.com
199.232.68.133 avatars1.githubusercontent.com
199.232.68.133 avatars2.githubusercontent.com
199.232.68.133 avatars3.githubusercontent.com
199.232.68.133 cloud.githubusercontent.com
140.82.113.6 api.github.com
```