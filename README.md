Git 基本指令（本地端）
====================
- 操作環境：
 - OSX 10.10
 - Git 2.5.1

- 指令步驟
	```shell
	git init # 初始化 git
	tree .git -al # 產生 .git 資料夾
	touch test.md # 產生 test.md 的空檔案
	tree .git -al # 新增檔案時 .git 沒有任何異動
	git add test.md # 新增 test.md 到暫存區
	tree .git -al # 會看見 .git/objectes 下多了檔案
	git commit # 把暫存區的所有檔案打包
	tree .git -al # .git/objectes 會多出兩個檔案
	echo 'test' >> test.md # 把 test 的字串寫入 test.md
	git add test.md # 新增檔案
	git commit -m 'Update' # 比較快速的 commit 方式
	```