#VideoPlayChecker
#影片播放檢查器

http://www.w3schools.com/tags/av_prop_paused.asp
可以用這個偵測影片是否在暫停狀態，再搭配個計時器，如果暫停中就不計時，這樣就可以知道使用者播放影片的總時間了

設定間隔時間需多長 (WaitTime)
影片開始：前台產生一組id 後端程式將該id寫入資料庫、開始時間、完成狀態  使用者 問卷編號 開始時間 結束時間
影片結束：結束播放後1分鐘，代表使用者閒置，將產生的id從資料庫刪除
作答去的檢查頁：是否有該code，且開始時間與結束時間間隔大於WaitTime，通過後將該code標示為完成，帶著該code進入作答內容頁
填寫完成作答內容：檢查該code是否為已完成，已完成才檢查作答是否正確