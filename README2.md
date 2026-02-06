1. Запуск бота в фоне
```
cd /root/bot
tmux new-session -s bot  # Создать сессию 'bot' в фоне
source venv_bot/bin/activate 
python bot.py

Ctrl+B -> D: выйти 
```

2. Проверка работы
```
tmux ls                    # Список сессий (должен показать 'bot: 1 windows')
tmux attach -t bot         # Подключиться к боту (увидите логи)
```

3. Основные команды
Запустить:	`tmux new  -s bot`

Посмотреть статус:	`tmux ls`

Подключиться:	`tmux attach -t bot`

Отключиться	`Ctrl+B → D`

Перезапустить:	`tmux kill -s bot + запуск заново`

Логи в реальном времени:	`tmux attach -t bot`


