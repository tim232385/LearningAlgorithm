# Stable Matching (Stable Marriage Problem)

又稱作穩定的婚姻問題(Stable Marriage Problem)，需同時達成``完全配對``與``穩定關係``，以婚友社為例：

### 完全配對
給定N個男人和N個女人，每個人須對所有異性進行喜好清單的排名，並且結婚。

### 穩定配對  
為了預防婚後出現婚外情，不能有兩個異性比他們的當前伴侶更喜歡對方，如果沒有這樣的人，這樣的婚姻關係就被視為穩定的。  

### 算法解決  
1.在第一輪中，每個男生對所有女生進行求婚，女生接受求婚後，狀態改為臨時訂婚。    
2.如果女生狀態為臨時訂婚，當求婚對象為更高優先序，高序的男生女生臨時訂婚對象改為高優先序 的男生，低序的男生向下一順位女生求婚。  
3.如果女生狀態為臨時訂婚，當求婚對象為更低優先序，低序的男生向下一順位女生求婚。  
  
## 喜好清單
![avatar](https://miro.medium.com/max/1280/1*mNtOmBvaWPI0h-ujmh2mNA.jpeg)
## 算法
![avatar](https://miro.medium.com/max/1280/1*4LMVIviLozFECMLkTHKZWQ.gif)

參考資料：  
[Wiki](https://en.wikipedia.org/wiki/Stable_marriage_problem)  
[Medium-UofCalifornia](https://medium.com/@UofCalifornia/how-a-matchmaking-algorithm-saved-lives-2a65ac448698)