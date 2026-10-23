# Данные FoxBot / FoxBot data

История цен, настройки и журнал покупок сохраняются на компьютере пользователя. Локальная панель и API используют loopback и ключ доступа. ESP32 обнаруживается и получает команды в локальной сети.

При запуске режима GenAPI системный промпт, сообщения, контекст команд и выбранные изображения передаются GenAPI по HTTPS. Используется собственный ключ пользователя, защищённый Windows DPAPI. Обработка переданных данных зависит от условий провайдера GenAPI. Не отправляйте изображения и тексты с личными данными, которые не хотите передавать провайдеру.

В приложении нет отдельной телеметрии разработчика. Публикуя issue на GitHub, не добавляйте API-ключи, пароли, журналы с личными данными и игровые скриншоты с приватной перепиской.

Price history, settings and purchase records stay on the user's computer. The local API requires a token. ESP32 discovery and control use the local network. In GenAPI mode, prompts, messages, command context and selected images are sent to GenAPI over HTTPS under the provider's policies. The API key is protected with Windows DPAPI. There is no separate developer telemetry. Do not post secrets or personal data in GitHub issues.
