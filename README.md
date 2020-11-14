git pull --rebase
	когда начинаем работу над своей локальной версией
		ребейс чтобы была чистая история от merges
git rm file.txt
git restore file.txt
git status - state of workind directory
git diff  - показывает изменения
	 Show changes between commits, commit and working tree, etc
git diff --staged
	показывает и новые появившиеся файлы (untracted)
git log 
	список всех коммитов
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