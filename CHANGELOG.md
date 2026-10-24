# Изменения / Changelog

## 0.2.0 — 2026-10-24

### Новое
- 44 общие API-команды: подготовка продажи, учёт затрат и работа с почтой.
- Долговечные черновики продажи с ценой, количеством, резервированием партии и прогнозом прибыли.
- Открытие почты после закрытия аукциона; чтение названия, количества и цены из письма покупки.
- Предварительное получение вложения отдельной командой: запись попытки до клика, защита от повторов и журнал результатов.

### Исправления
- OCR мелких цифр цены письма: проверка согласованности на двух масштабах. На предоставленных снимках корректно читаются 4 серебра 10 меди.

### Важно
- Выставление лотов и получение выручки пока отсутствуют. Фактическая прибыль неизвестна.
- Получение вложений предварительное: исчезновение из письма не подтверждает поступление в рюкзак. Проверка на реальной игре после получения ожидает снимка; неопределённая попытка блокирует следующие получения.
- Автоматический режим остаётся заглушкой. Сквозная проверка торговли через ESP32 и платных запросов GenAPI не выполнена.
- Установщик Windows x64 без цифровой подписи, обновление вручную. Исходники приватны.

### English
- 44 shared API commands, persistent sale drafts, cost tracking and profit estimates.
- Open mail after closing the auction; read purchase letters and their item, quantity and price.
- Preliminary attachment collection with a durable pre-click journal and duplicate protection.
- Fixed small price-digit OCR with agreement checks at two scales.
- Game sale execution and proceeds collection are not implemented. Inventory delivery is not verified; live post-collection validation is pending. Unknown collections block further collection. Automatic mode is a placeholder.
- Unsigned Windows x64 installer; manual updates. Source code remains private.

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
