---
tags:
- разработка
- лаба
---

1. зарегистрироваться [здесь](https://github.com/) (думаю сами справитесь)  
2. Создать репозиторий  
![](../Files/Pasted%20image%2020210913181617.png)  
3. назвать репозиторий и создать его  
![](../Files/Pasted%20image%2020210913181940.png)  
4. качаете git [тык](https://git-scm.com/download/win) (просто тыкаете далее)
5. заходите в папку проекта -> ПКМ -> Git Bash Here
6. настраиваем логин и почту (кавычки не убирать)
p.s. копировать(Ctrl + Insert) вставить(Shift + Insert)
```bash
	git config --global user.name "Ваш логин при регистрации"
	git config --global user.email "Ваша почта при регистрации"
```
7. Инициализируете проект (добавляете файлы необходимые для git)
```bash
	git init
```
7. добавляете новые файлы в систему git (для гита ваши файлы проекта новые)
```bash
	git add .
```
8. создание коммита (сделать сохранение как в играх)(кавычки не убирать)
```bash
	git commit -m "Название коммита желательно на английском"
```
9. у github есть ветки, и нужно выбрать нужную - главную
```bash
	git branch -M main
```
10. теперь нужно соединить локальный репозиторий (нашу папку) с репозиторием в github
```bash
	git remote add origin https://github.com/sug111/test.git
```
p.s. все команды есть при создании репозитория, просто скопируйте свою команду  
![](../Files/Pasted%20image%2020210913184555.png)  
11. отправляем изменения на github
```bash
	git push -u origin main
```
- логинимся через браузер  
![](../Files/Pasted%20image%2020210913191000.png)  
![](../Files/Pasted%20image%2020210913191134.png)  
12. перезагрузите страницу с github
## готово, вы молодцы)

>p.s. забыл про авторизацию через браузер (другие способы ssh и токен)
