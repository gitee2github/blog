+++
title = "Guidance"

+++
## 前期准备

1. 注册码云账号，请参考[http://git.mydoc.io/?t=179267](http://git.mydoc.io/?t=179267)。
2. 设置主邮箱，进入邮箱页面[https://gitee.com/profile/emails](https://gitee.com/profile/emails)配置个人主邮箱。
3. 签署CLA，进入CLA签署页面[https://openeuler.org/zh/cla.html](https://openeuler.org/zh/cla.html)，填写必填信息签署CLA。
4. 准备GIT环境，详细参见：[http://git.mydoc.io/?t=180692](http://git.mydoc.io/?t=180692)。

## 编写博客内容

博客采用MD（markdown）格式编写、组织内容，博客内容由两部分组成，博客描述信息和博客内容，其中博客描述信息包含如下几部分：
-   banner: 一个用于呈现博客内容简要的图片，这个图片将会在博客列表中显示出来。
-   title: 博客标题。
-   summary: 博客内容的精简描述。
-   author: 该博客的作者。
-   tags: 博客的标签
-   archives: 该博客发布的年月份，用于首页上的分类显示。
-   date: 博客发布日期。

样例如下：

```
+++
banner = "img/banners/banner-1.jpg"
title = "openEuler 线下活动介绍"
date = "2019-10-10"
tags = ["meetup"]
archives = "2019.10"
author = "user1"
summary = "openEuler第一次线下活动将在北京举行。"
+++
此处为博客内容.
```

## 上传博客

博客系统采用码云的PR模式上传（提交）博客，步骤如下：
1. Fork 博客工程[https://gitee.com/openeuler/blog](https://gitee.com/openeuler/blog), Fork方法参见[http://git.mydoc.io/?t=153749](http://git.mydoc.io/?t=153749)。
2. 使用git，在本地机器上clone 码云上fork出来的工程。

```
git clone https://gitee.com/<your-id>/blog
```

4. 创建git分支

```
git checkout -b <branch-name>
```

6. 将博客内容放置在content\post目录下。
7. 保存到git并提交到码云

```
git add <file-path>
git commit -m "<message>"
git push origin <branch-name>:<branch-name>
```

8. 创建PR，详细参见[http://git.mydoc.io/?t=153749](http://git.mydoc.io/?t=153749)

--