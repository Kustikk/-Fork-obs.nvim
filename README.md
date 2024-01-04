This repository is a fork [obs.nvim](https://github.com/IlyasYOY/obs.nvim)

### The following changes have been made here:
- Изменёна обработка пути до папки с шаблоном дня, реализована через относительный путь (Переменной vault_home)
Пример реализации
```lua
    vault_home = "~/Obsidian/Obsidian journal TestNvim",
    journal = {
        template_name = "📆 Daily", -- Шаблон для ежедневной заметки
    },
    journal_home = "📌 Periodic/📆 Daily", -- Путь до Daily notes
    templates_home = "🛠 Templates/", -- Путь до шаблонов
```

- Добавлены несколько сокращённых форматов даты и времени
>[!NOTE]
>
>{{date:DM}} - `0401` 04/day, 01/month
>
>{{date:dd}} - `Чт` Сокращение дня недели
>
>{{time}} - `10:30` Час:Минуты
>
>{{time:x}} - `1704373114` Timestamp
