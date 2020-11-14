```
index directory/working directory/repository

git commit INFO.md -m 'update INFO.md'   +
git add .								 -
git commit -am 'do something'		     -
git add -i							     +
		конкретный кусок файла добавить в индекс
	
git pull --rebase
	когда начинаем работу над своей локальной версией
		ребейс чтобы была чистая история от merges
git rm file.txt
git add добавить фаил в индекс
git restore file.txt  отмена действия внутри рабочей директории(к прежнему сост.)
	--staged  отменить добавленное в индекс
git status - state of workind directory *
git diff  - показывает изменения
	 Show changes between commits, commit and working tree, etc
git diff --staged
	показывает и новые появившиеся файлы (untracted) *before commit
git log 
	список всех коммитов
	--oneline сокращенный вывод
	--graph
git log -p
	дополнительно выводит diff для каждого коммита
	f - вперед, u - назад
git show %commit_hash%
	все изменения врамках коммита
git blame path/file
	все изменения в конкретном файле(когда/какой комит)
git grep str
	ищет строку по всему проекту
	-i без учета регистра
git clean -fd удалить все untracked files(неотслеживаемые)
	-f -force, -d -directory
git revert %commit_hash%	
	новый коммит инвертирующий изменения коммиту, /безопас отмена/
git reset HEAD~   
	откатит последний коммит в рабочую директорию
	HEAD~2 - 2 последних коммита...
	--hard
		удалить последний коммит, без сохранения в истории /dangerous/
		использ только локально
git commit --amend		--поправить
	изменение последнего локального коммита(откат в рабочий+новый коммит)
git checkout %commit_hash%	/ %branch_name% -b create
git switch -
git show
git stash   добав и восстанов идет из стека
	working+index->stash
	не задевает новые фаилы
git stash pop
linux:	
	echo 'flush file' > README.md
	echo 'to new line' >> INFO.md
	rm file - remove file
	mv file /tmp - move file
	mv file file2 - rename file
vi:
	a A, after cur, end line
	i I, insert before cur, start
	wq
	q! - no save
	x X - del char, reverse
	dd строку D удалить спарва от курсора
	r заменить символ
	yy копия строки
	yw копия слова
	p вставить буфер
	j удалить переход строки
```