# Planner-Cat 🐱

Планировщик задач с анимированным котом!

## Как собрать приложение

### Способ 1: GitHub Actions (САМЫЙ ПРОСТОЙ)

1. Создай новый репозиторий на [GitHub](https://github.com/new)
2. Загрузи все файлы из этого архива в репозиторий
3. Перейди во вкладку **Actions** → **Publish** → **Run workflow**
4. Жди 5-10 минут
5. Перейди во вкладку **Releases** — там будут `.exe`, `.dmg`, `.AppImage`

### Способ 2: Собрать локально

**Windows:**
```bash
# Установи Rust (один раз)
https://rustup.rs/

# Установи Tauri CLI
cargo install tauri-cli

# Собери приложение
cd src-tauri
cargo tauri build
```

**Mac/Linux:**
```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
cargo install tauri-cli
cd src-tauri
cargo tauri build
```

Готовое приложение будет в `src-tauri/target/release/bundle/`

## Возможности

- 📅 Календарь с задачами
- ✅ Автосортировка (выполненные вниз)
- 🔄 Повторяющиеся задачи
- 🏷️ Теги и фильтры
- 🐱 Анимированный кот, реагирующий на продуктивность
- 💾 Данные хранятся в файле (не в браузере!)
