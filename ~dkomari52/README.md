В корневой папке проекта выполнить следующие команды
git init - инициализация(создание) репозитория
    Создаем .gitignore - прописывая в него файлы и папки, которые не должны попасть в репозиторий.
	Минимальные настройки git’а:
git config --global user.name "username"
git config --global user.email "you@mail.ru"
git add . - добавляем все файлы проекта(кроме тех, что в .gitignore). Подготавливаем файлы к коммиту(сохранению)
git commit -m “комментарий к коммиту”  - делаем коммит(сохраняем текущее состояние файлов в репозитории)
Каждый раз, когда вам нужно сохранить изменения в локальном репозитории выполните:
git add .
git commit -m “комментарий к коммиту”

При создании репозитория из командной строки делаем так:
echo "# Docker" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M master
git remote add origin git@github.com:mariako25/dkomari52.git
git push -u origin master

При наличии существующего репозитория - так:
git remote add origin git@github.com:mariako25/dkomari52.git
git branch -M master
git push -u origin master

    ПОТОМ СОЗДАЕМ ВИРТУАЛЬНОЕ ОКРУЖЕНИЕ:
python3 -m venv .venv
source .venv/bin/activate
