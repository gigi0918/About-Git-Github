```bash
# 創建目錄
mkdir ptc_git

# 進到目錄中
cd ptc_git

# add git (初始化)
git init

# 檢查是否有成功將 hello 寫入檔案
cat hello.txt

# 將 hello! 寫入(>覆蓋式)檔案 hello.txt
echo hello! > hello.txt

# 檢查是否有成功創建檔案
ll

# 檢查是否有成功寫入檔案
cat hello.txt

# 查看狀態
git status

# 加入 staging 區域
git add .

# 加入至 git dir
git commit -m "add hello! to hello.txt"

# 創建分支 dev
git branch dev

# 切換分支
git checkout dev

# 檢查原始檔案內容
cat hello.txt

# 將 Ruby! 寫入(>> 末端寫入)檔案 hello.txt
echo Ruby! >> hello.txt

# 檢查是否有成功寫入檔案
cat hello.txt

# 查看狀態
git status

# 加入 staging 區域
git add .

# 加入至 git dir
git commit -m "add Ruby! to hello.txt"

# 查看狀態
git status

# 查看 log 
git log --oneline

# 切換回 master 分支
git checkout master

# 檢查原始檔案內容
cat hello.txt

# 合併分支
git merge dev

# 檢查原始內容 如果輸出 hello! 換行(\n) Ruby! 表示合併成功！
cat hello.txt

```