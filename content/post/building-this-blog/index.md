---
title: Building This Blog
date: '2022-05-22T00:00:00Z'
summary: How to build this website and the problem encounter while doing so.

# View.
#   1 = List
#   2 = Compact
#   3 = Card
view: 2

categories:
  - website




# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Placement options: 1 = Full column width, 2 = Out-set, 3 = Screen-width
# Focal point options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
image:
  placement: 1
  caption: ''
  focal_point: ""
  preview_only: false
---
## 如何架設本站

本站參考的是這篇文章:[**點我**](https://azurerain.xyz/category/website/)
，從Part1到Part5做完即可。
***
## 遇到問題
1.在根據文章來啟動本地server時，遇到powershell報錯: <br>
```
Error: failed to download modules: exec: "go": executable file not found in $PATH
```
💡**解決**:  
參照wowchemy的網站:[**點我**](https://wowchemy.com/docs/guide/troubleshooting/#error-go-executable-not-found) <br>
在**不以**工作管理員執行的情況下打開powershell，輸入:<br>
``` 
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
iwr -useb get.scoop.sh | iex
```
如果有詢問Do you want to change the execution policy?的話，按下Y和enter。
完成後再輸入
```
scoop install git go hu go-extended
```
即可解決。
***
## 延伸
- [Markdown語法](https://keatonlao.gitee.io/a-study-note-for-markdown/syntax/#%E6%B0%B4%E5%B9%B3%E5%88%86%E9%9A%94%E7%BA%BF)
