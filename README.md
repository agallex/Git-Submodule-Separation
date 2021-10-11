# Instruction
Клонирую репозиторий свой:

git@github.com:agallex/Git-Submodule-Separation.git

Потом клонирую репозиротирий с проектом:

git@github.com:tensorflow/tensorflow.git

cd tensorflow

Оставляю все нужное в репозитеории с проектом:

git filter-branch --subdirectory-filter tensorflow/contrib -- --all

Все в папочку обратно кидаю для красоты:

mkdir contib

mv * contib

Коммичу все, затем добавляю удаленный репозиторий и закидываю туда все изменения:

git add .

git commit -m "sd" 

git remote add main "git@github.com:agallex/Git-Submodule-Separation-Public2.git"

git push -u main r1.14

Теперь в репозитории Git-Submodule-Separation-Public, я создаю ссылку на Git-Submodule-Separation-Public2:

git submodule add "git@github.com:agallex/Git-Submodule-Separation-Public2.git"

git add --all

git commit -am «lll"

git push origin
