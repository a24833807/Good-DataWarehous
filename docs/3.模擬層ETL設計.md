# 使用Kettle 設計Stagging ETL轉檔

目前核心層已有資料，需將核心層資料拋轉至模擬層。

## 1.取得核心層的Delta Date:

因為stagging層採Delta Load，所以需要抓核心層Date(註解)

<img width="1312" height="908" alt="image" src="https://github.com/user-attachments/assets/cac27a42-9e7a-4b6c-a4e0-0436b7f8e336" />

實際上第一次stagging 已Full Load為主:

<img width="892" height="680" alt="image" src="https://github.com/user-attachments/assets/bda96c01-0ae7-4c69-b9f1-0f93cd0aca95" />


## 2.設定日期格式:

將原先的String 轉成TimeStamp 並且設定好日期格式(YYYY-mm-dd hh:mm:ss)

<img width="1312" height="770" alt="image" src="https://github.com/user-attachments/assets/50b266d8-ea79-4144-bac7-48644784739b" />

## 3.儲存變數:

將設定好的值儲存成後續要用的變數(LastLoadDate)
<img width="1316" height="912" alt="image" src="https://github.com/user-attachments/assets/1f949c52-62a3-4ec7-ad55-b8f2947bd5cd" />

## 4.取得變數:

<img width="1308" height="911" alt="image" src="https://github.com/user-attachments/assets/8e5fe324-d29d-41e7-927b-df1bc9a6359d" />

## 5.將變數用於篩選條件，匯出資料

<img width="887" height="675" alt="image" src="https://github.com/user-attachments/assets/c29d1b3b-c632-4d1f-ada9-f10953f49269" />

