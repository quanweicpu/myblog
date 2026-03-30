

  

## 🧱 1. 安装 PowerShell 7（pwsh）

  

### ✅ 推荐方式（winget）

1. 打开终端（Win + X → Terminal）

2. 执行：

winget install --id Microsoft.PowerShell --source winget

3. 安装完成后重启终端

  

---

  

## 🚀 2. 打开 PowerShell 7

  

方法：

- Win 键搜索 PowerShell 7

- 或 Win + R 输入 pwsh

  

验证：

$PSVersionTable.PSVersion

Major = 7 即成功

  

---

  

## ⚙️ 3. 安装 Hugo

  

下载：

https://github.com/gohugoio/hugo/releases

  

步骤：

1. 下载 hugo_extended_xxx_windows-amd64.zip

2. 解压得到 hugo.exe

3. 放入 C:\hugo\

4. 添加到 PATH

  

验证：

hugo version

  

---

  

## 🏗️ 4. 初始化 Hugo 站点

  

cd D:\blog\

hugo new site myblog

cd myblog

  

目录说明：

- hugo.toml 配置文件

- content 文章目录

- themes 主题目录

  

---

  

## 🎨 5. 安装主题（hugo-book）

  

git clone https://github.com/alex-shpak/hugo-book themes/hugo-book

  

编辑 hugo.toml：

theme = "hugo-book"

  

---

  

## 🌐 6. 本地运行

  
cd D:\blog\myblog

hugo server -D

  

访问：

http://localhost:1313/

  

---

  

## 🧠 7. Obsidian 联动

  

打开 Vault：

D:\blog\myblog\

  

在 content 下写文章：

  

---

title: "My First Post"

date: 2026-03-23

---

  

Hello Hugo + Obsidian 🚀

  

---

  

## 📤 8. Git 推送

  

cd D:\blog\myblog

  

git add . 

git commit -m "update content" 

git push origin main

  

---

  

## ✅ 总流程

  

1. 安装 PowerShell

2. 安装 Hugo

3. 创建站点

4. 安装主题

5. 用 Obsidian 写内容

6. 本地预览

7. 推送上线