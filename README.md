# sete
# Создание папки и клонирование репозитория
mkdir git_lab1_lesson2
cd git_lab1_lesson2
git clone https://github.com/YandexLyceum/human.git
cd human

# Просмотр веток и файла human.txt
git branch -a
cat human.txt

# Сравнение веток
git diff master boots
git diff master buttons
git diff boots buttons

# Создание и слияние веток
git checkout master
git branch boots_buttons
git checkout boots_buttons
git merge boots
git merge buttons

# Проверка конфликтов и переключение на master
git checkout master

# Выкладывание на ваш гитхаб
git remote add origin_mine https://github.com/k7ndcat/sete.git
git push -u origin_mine master
