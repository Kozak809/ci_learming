# CI Learning

Учебный репозиторий для изучения настройки Continuous Integration (CI) с использованием GitHub Actions и тестирования на Python с помощью `pytest`.

## 📁 Структура проекта

* `calculator.py` — простой калькулятор (сложение, вычитание, умножение, деление).
* `test_calculator.py` — тесты для калькулятора с использованием `pytest`.
* `greeter.py` — функция приветствия.
* `test_greeter.py` — тесты для функции приветствия.
* `requirements.txt` — зависимости проекта (`pytest`).
* `.github/workflows/ci.yml` — конфигурационный файл GitHub Actions для автоматического запуска тестов при коммитах и пулл-реквестах.

---

## 🛠️ Установка и локальный запуск

1. Убедитесь, что у вас установлен **Python 3.11+**.
2. Установите зависимости:
   ```bash
   pip install -r requirements.txt
   ```
3. Запустите тесты локально:
   ```bash
   pytest
   ```

---

## 🚀 Настройка Continuous Integration (CI)

Проект настроен на автоматическое тестирование с помощью **GitHub Actions**. Конфигурация находится в файле [`.github/workflows/ci.yml`](file:///c:/Users/Kozak/Desktop/ci_learming/.github/workflows/ci.yml).

При каждом `push` в репозиторий или открытии `pull request` автоматически запускается виртуальная машина Ubuntu, которая:
1. Клонирует репозиторий.
2. Настраивает окружение Python 3.11.
3. Устанавливает `pytest`.
4. Запускает тесты.
