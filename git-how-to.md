# Как пользоваться git
Git -- распределенная система контроля версий.

## Основные команды
Добавить файлы в коммит: 
```
git add <paths>
```
Сделать коммит:
```
git commit -m <message>
```
Сделать пуш:
```
git push
```

## SSH
SSH ключ создается локально. Для Linux:
```
ssh-keygen -t ed25519 -C <your_email@example.com>
```
Далее нужно следовать инструкциям `keygen`, он предложит создать пароль.
Потом добавляем ключ:
```
ssh-add ssh_key
```
Копируем содержимое публичного ssh-ключа в буфер обмена.
```
cat ssh_key.pub
# Копируем 
```
Переходим в Github > Profile > Settings > SSH, вставляем содержимое, добавляем SSH-ключ.
