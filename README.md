# Google 表單串接

## 相關連結

* [表單問卷](https://forms.gle/xF5HbtV6NZHwsscj6)
* [回應表單](https://docs.google.com/spreadsheets/d/18svFd6su5DzqQbgLWKEjJeC_i4iw4CjBoogfWr6Dvz8/edit?resourcekey#gid=164086538)

## 實作方式

* 建立問卷，問卷欄位需與版面欄位一致
* 填寫問卷欄位不提交（幫助辨識欄位名稱），開啟開發者工具
* 找到 `<form>` 標籤的 action url，即為請求網址
* 找到 div 內有所有為 hidden 的 input，將 `entry.*` 對應至版面的相應欄位 name 屬性
* input:checkbox 加上 value 值