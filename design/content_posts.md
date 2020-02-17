# Posts
This file is to explain in which way the content of the blogs are stored and readed by the blog system.

## What is supported in the blog
A blog can include many format of information, like text, pictures, videos, annimations or others. 

openEuler Blog is designed to support the following formats:

1. text
2. static picture
3. links

## Folder design
The content of blogs are under ./content

```
|__ _draft       --list the cases of blogs 
|__ guidance     --house the guidance to post and maintain the blogs
|__ post         --house all the final posts
   |__ yyyymmdd  --house the blogs by months, such as 202002
```

## Post content design
### File name
To create a post, add a file to your _post/yyyymmdd/_ directory with the following format:

```
YEAR-MONTH-DAY-title.MARKUP
```
Where YEAR is a four-digit number, MONTH and DAY are both two-digit numbers, and MARKUP is the file extension representing the format used in the file. For example, the following are examples of valid post filenames:
```
2020-01-01-new-years-is-coming.md
2020-02-15-how-to-write-a-blog.md
```

If you need add images to your post, please name the images as 
```
YEAR-MONTH-DAY-title-NN.MARKUP
```
Where the YEAR, MONTH, DAY, and title are the same as your blog file, and NN is the serial number of the pictures, like 01, 02 and so on. The MARKUP is the file extension, and for pictures it is recommended to use png.
The following are one example.
```
2020-01-01-new-years-is-coming.md
2020-01-01-new-years-is-coming-01.png
2020-01-01-new-years-is-coming-02.png
```

### File headers
Functionally, the post should support categories, archives, title, date, brief description, thus the file headers should be as below.
```
+++
title = ""
date = "yyyy-mm-dd"
tags = ["aaaa", "bbbb", "cccc"]
archives = "yyyy-mm"  //by months
author = "name of author"
summuary = ""
+++
```
