# Задание 1: Определение оболочки по умолчанию
Команда: grep ^max /etc/passwd
Результат: max:x:1000:1000:Max,,,:/home/max:/bin/bash
Сохранено в: max_shell

# Задание 2: Изменение оболочки пользователя
Команда: sudo usermod -s /bin/sh max
Результат: Оболочка изменена для пользователя max
Сохранено: Содержимое /etc/passwd в файл passwd

# Задание 3: Добавление переменной среды
Команда: echo 'export ENVIRONMENT=Dev' >> /home/max/.profile
Сохранено: Обновлённый ~/.profile в файл profile

# Задание 4: Создание алиаса
Команда: echo 'alias cur="date"' >> /home/max/.profile
Сохранено: Обновлённый ~/.profile в файл profile

# Задание 5: Изменение приглашения оболочки
Команда: echo 'PS1="[\\d]\\u@ws01 "' >> /home/max/.profile
Результат: Приглашение установлено в [Sun Nov 28]max@ws01
Сохранено в: prompt

# Задание 6: Вывод точного времени изменения файла
Команда: ls -l --time-style=full-iso
Сохранено в: ls
 