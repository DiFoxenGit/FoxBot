# Изменения / Changelog

## 0.1.0 — 2026-10-23

Первый выпуск для Windows x64.

- Автопоиск ESP32 и управление мышью и клавиатурой по протоколу MouseKey.
- Поиск аукциона и предметов, OCR первой страницы, история цен, список отслеживания и очередь парсера.
- Локальная веб-панель, экспорт CSV/JSON и API из 31 команды.
- Режим бота с отдельными командами поиска, выбора лота, количества, покупки и проверки списания.
- Баланс с обновлением после покупки; журнал сделок и защита от повторного подтверждения.
- GenAPI: чат, системный промпт, изображения, выбор действий моделью и бюджет покупок.
- Автоматический режим пока является заглушкой.

Ограничения: профиль русского аукциона при масштабе 100%; реальная покупка и платный запрос GenAPI не проверялись. При неоднозначном списании новые покупки блокируются. Установщик без цифровой подписи; автоматического обновления нет.

### English

First Windows x64 release: ESP32 discovery and input, auction OCR and price history, watchlist parser, local dashboard and 31 API commands, separate purchase/quantity/verification commands, balance tracking, and GenAPI chat with model-selected actions and purchase budgets.

The automatic mode is a placeholder. Russian auction UI at 100% scale is the initial recognition profile. Live purchases and paid GenAPI requests have not been validated. Ambiguous debits block further purchases. The installer is unsigned; updates are manual.
