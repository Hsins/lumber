## 情境一：一開始就打算後台運行
	- 使用終端複用器（Terminal Multiplexer）如 `screen`, `tmux`, `nohup`, `byobu` 等
## 情境二：一開始沒打算後台運行
	-
	  1. 按下 <kbd>CTRL+Z</kbd> 讓進程進入掛起（Suspend）狀態
	-
	  2. 終端會返回如 `[NUM]+ Stopped COMMAND` 的輸出
	-
	  3. 使用命令 `bg &NUM` 會讓掛起的進程在後台運行
	-
	  4. 執行 `disown` 解除當前 SHELL 與該進程的所屬關係
	- [備註] 可以使用 `job` 命令檢查任務列表
## 參考資料
	- [Linux 在終端打開程序後關閉終端，程序也跟著關閉了怎麼辦？ | 知乎](https://www.zhihu.com/question/442188249)
	-