
## 1. 创建一个空目录
```bash
$ mkdir repository
$ cd repository
```
## 2. 把目录变成git仓库
```bash
$ git init
Initialized empty Git repository in C:/Users/uidw3549/Git/02.Github Repository/repository/.git/
```
## 3. 编写新文件
```bash
$ echo "this is readme file" > readme.txt
$ ls
readme.txt
```
## 4. 添加文件到仓库
   - 添加文件到[暂存区](/staging)
    
    ```bash
	$ git add readme.txt 
    ```
    
   - 查看仓库状态
   ```bash
	$ git status
	On branch master
	Initial commit
	Changes to be committed:
		(use "git rm --cached <file>..." to unstage)
		   new file:   readme.txt
   ```
   - 提交到仓库
   ```bash
   $ git commit -m"create readme.txt"
   [master (root-commit) d9abbb7] create readme.txt
    1 file changed, 1 insertion(+)
    create mode 100644 readme.txt
   ```
   - 再查看文件状态,文件已经提交到仓库中
   ```bash
   $ git status
On branch master
nothing to commit, working tree clean
   ```

***
* ``` $ git init ``` 创建创建仓库
*  ``` $ git add <file> ``` 添加文件到暂存区
*  ``` $ git commit -m <message> ``` 提交到仓库
*  ``` $ git status ``` 查看仓库状态
