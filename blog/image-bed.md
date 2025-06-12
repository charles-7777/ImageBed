+++
date = '2025-06-12T19:33:46+08:00'
title = 'Github + PicGo 搭建图床'

+++

1.github 创建public仓库用来存放照片

---

![image-20250612194003078](C:/Users/charles/AppData/Roaming/Typora/typora-user-images/image-20250612194003078.png)

2.创建token

---

token将来PicGo操作你的github仓库来上传图片时要用到，在 GitHub 账户下 `Setting - Developer setting - Personal access tokens(classic)` 下创建一个不过期(no expiration)的 Token，权限需要开启 `repo`.这个我们在用Github action 来部署博客仓库时已经创建了，用那个就好.token 在创建时只显示一次，要保存好哦！

![image-20250612194911382](C:\Users\charles\AppData\Roaming\Typora\typora-user-images\image-20250612194911382.png)

3.配置PicGo

###github 搜索[PicGo][Molunerfinn/PicGo: :rocket:A simple & beautiful tool for pictures uploading built by vue-cli-electron-builder](https://github.com/Molunerfinn/PicGo) 然后安装

###图床具体参数配置

![image-20250612195909612](C:\Users\charles\AppData\Roaming\Typora\typora-user-images\image-20250612195909612.png)

```
仓库名 分支名 对应于之前你创建的GitHub仓库
Token就是前面创建的Token,被PicGo用来上传照片到长仓库
路径可以自定义
自定义域名格式:https://cdn.jsdelivr.net/gh/用户名/仓库名@分支名
```

4.[Typora](https://github.com/shuhongfan/TyporaCrack)

Typora 可搭配PicGo使用

![image-20250612201005537](C:/Users/charles/AppData/Roaming/Typora/typora-user-images/image-20250612201005537.png)

