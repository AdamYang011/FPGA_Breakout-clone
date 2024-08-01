# FPGA打磚塊小遊戲
此遊戲參考自著名的遊戲BBTan, 並以此進行改動
利用FPGA上的8*8 LED矩陣作為打磚塊的顯示畫面, 七段顯示器用來顯示當前關卡, LED 陣列用來顯示發球路徑及球數, FPGA上的按鈕則用來操控移動跳板與切換發射路徑

打磚塊的顯示畫面 & 顯示當前關卡:

<img src="https://github.com/user-attachments/assets/7f433100-4e32-4643-b485-aaae0557a1db" width="30%"><img src="https://github.com/user-attachments/assets/bb745f9f-bdab-4bdd-8c1a-b6949a282757" width="30%">

顯示發球路徑及球數 & 移動跳板按鈕與發射路徑調整按鈕:

<img src="https://github.com/user-attachments/assets/52e93f33-05f4-49a1-a7e8-717d9dd3bfa7" width="30%"><img src="https://github.com/user-attachments/assets/6eb149cb-0073-43f1-83cb-7f0f3407377d" width="30%">

遊戲規則說明:
1.	LED矩陣最後一行為跳板移動位置, 當上方磚塊壓下來直到跳板前一條時，即視為遊戲失敗
2.	初始球數共有兩顆, 隨著關卡推進, 將逐步增加球數
3.	當球碰到方塊和範圍邊線時將進行反彈
4.	上方移動的方塊共有兩種顏色, 綠色需要擊打兩次才會消除, 青色擊打一次即可
5.	共有四個按鈕, 兩個按鈕作為跳板左右的移動, 一個按鈕用來調整發射方向
6.	隨著關卡推進, 方塊擊打難度將逐步提高
