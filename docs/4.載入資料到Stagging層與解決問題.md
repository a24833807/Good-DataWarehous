## 載入資料到Stagging層


# 1.將前述的GETDataDate、SetSaleData加入到JOB裡面
<img width="1323" height="912" alt="image" src="https://github.com/user-attachments/assets/fb9795cb-20b5-4e1e-b1a3-b4ec60cf3c85" />

# 2.調整SetSaleData 
加入Table output流程，將資料匯出至Stagging的Sale資料表
<img width="868" height="658" alt="image" src="https://github.com/user-attachments/assets/fcdeb1a0-e898-4ef1-9cf1-6c7a45079397" />

# 3.調整Mapping欄位設定
勾選Specify database field
<img width="867" height="661" alt="image" src="https://github.com/user-attachments/assets/eb9e4faa-1ab4-4c02-92ce-df9aa2ae565a" />

將源頭欄位設定調整成目標表欄位。
<img width="877" height="660" alt="image" src="https://github.com/user-attachments/assets/e67ae468-1c66-4c13-91aa-e140137e2ce3" />


