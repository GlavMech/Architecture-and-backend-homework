# Architecture-and-backend-homework

# Выполнено:
1. Склонирован репозиторий проекта к себе на компьютер.
2. Установил менеджер пакетов uv
3. Установил зависимости проекта: uv sync
4. Создайл свою конфигурацию ruff используя pyproject.toml.
   ```python
   [tool.ruff]
      line-length = 120

   [tool.ruff.lint]
      select = ["E", "F", "W"]
      ignore = ["E501"]
      exclude = ["migrations/", "tests/", "venv/"] ```



# Анализ и форматирование кода:
 - ruff check .  — для анализа кода и выявления проблем.
 - ruff format . — для форматирования

В коде были выявлены многие ошибки.
Были исправлены таки записи как:
- Заменены неявные сравнения
   - == None → is None
   - == True → просто if ...
   - == False → if not ...
- Были удалены множество неиспользуемых переменных.
- Добавлены недостающие импорты.
- Исправлены синтаксические ошибки.
