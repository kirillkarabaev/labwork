

## 1. Создание аккаунта на сайте GitHub
- Перейдите на [GitHub](https://github.com/) и зарегистрируйте новый аккаунт, заполнив все необходимые поля.

## 2. Сделать копию в личное хранилище из https://github.com/Kurtyanik/LR6/ (Fork)
- Перейдите на страницу репозитория [Kurtyanik/LR6](https://github.com/Kurtyanik/LR6/).
- Нажмите на кнопку `Fork` в правом верхнем углу страницы.
- Выберите свой аккаунт для создания форка.

## 3. Установить Git
- Перейдите на [страницу загрузки Git](https://git-scm.com/) и установите Git, следуя инструкциям для вашей операционной системы.

## 4. Настроить клиент Git
Откройте терминал и выполните следующие команды, введя своё имя и email
## 5. Клонировать свой личный удалённый репозиторий на компьютер
- Получите URL вашего репозитория, он может выглядеть так: `https://github.com/kirillkarabaev/LR6.git`.
- Выполните команду в терминале:
- git clone https://github.com/kirillkarabaev/LR6.git
- ## 6. Добавить файл через интерфейс GitHub и подтянуть изменения в локальный репозиторий
- В своём репозитории на GitHub нажмите на кнопку `Add file` → `Upload files` и добавьте файл.
- После этого выполняйте:
-  Или git pull origin master
-  ## 7. Получить историю операций для каждой из веток
- Для получения истории можно использовать команду:
-  git log --oneline --graph --all
-  ## 8. Выполнить слияние в ветку master, разрешив конфликт
- Переключитесь на ветку `master`:
- git checkout master
- - Выполните слияние и решите возможные конфликты:
  - git merge main
  - git add .
git commit -m "Разрешены конфликты и выполнено слияние"
## 9. Удалить побочную ветку после успешного слияния
- Убедитесь, что вы находитесь на ветке `master`, затем выполните:
- bash
git branch -d имя_ветки
## 10. Сделать изменения и зафиксировать их, оставляя комментарии, несколько раз
- Внесите изменения в файлы, затем выполните:
- git add .
git commit -m "Описание изменений"
- Повторите этот шаг несколько раз.

## 12. Сделать откат коммита
- Для отката последнего коммита:
- git revert HEAD
