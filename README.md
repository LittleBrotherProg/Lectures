<style>
:root {
  --bg:       #0d1b2a;
  --bg2:      #1a2a3a;
  --bg3:      #0a1628;
  --accent:   #1b91ff;
  --orange:   #e07b39;
  --green:    #2fca72;
  --gold:     #f0c040;
  --text:     #c8d8e8;
  --text2:    #8ab4d4;
  --border:   #1b3a5c;
  --code-bg:  #1e2d3d;
  --code-fg:  #7fdbca;
  --red:      #e05555;
}
body, .jp-RenderedHTMLCommon {
  background: var(--bg) !important;
  color: var(--text) !important;
  font-family: 'Segoe UI', Arial, sans-serif !important;
}
h1,h2,h3,h4 { color: #ffffff !important; }
h1 { border-bottom: 2px solid var(--accent) !important; padding-bottom: 8px !important; }
h2 { color: var(--accent) !important; }
h3 { color: var(--text2) !important; }
a  { color: var(--accent) !important; }
code {
  background: var(--code-bg) !important;
  color: var(--code-fg) !important;
  padding: 2px 6px !important;
  border-radius: 4px !important;
}
pre code { padding: 0 !important; }
pre {
  background: var(--code-bg) !important;
  border-left: 3px solid var(--accent) !important;
  border-radius: 6px !important;
  padding: 14px 18px !important;
}
table { border-collapse: collapse !important; width: 100% !important; }
th {
  background: var(--bg3) !important;
  color: var(--accent) !important;
  border: 1px solid var(--border) !important;
  padding: 8px 12px !important;
}
td {
  border: 1px solid var(--border) !important;
  padding: 8px 12px !important;
  color: var(--text) !important;
}
tr:nth-child(even) td { background: var(--bg2) !important; }
blockquote {
  border-left: 4px solid var(--gold) !important;
  background: #1a2a1a !important;
  padding: 10px 16px !important;
  border-radius: 0 8px 8px 0 !important;
  color: var(--text) !important;
}
</style>

<div style="background:linear-gradient(135deg,#1a2332 0%,#0d1b2a 100%);border-radius:16px;padding:40px 36px;margin-bottom:24px;">
  <div style="color:#8ab4d4;font-size:13px;font-weight:600;letter-spacing:3px;text-transform:uppercase;margin-bottom:8px;">Подготовка к экзамену</div>
  <div style="color:#ffffff;font-size:32px;font-weight:900;margin-bottom:8px;">🎓 Разбор заданий ЕГЭ<br>по информатике</div>
  <div style="color:#8ab4d4;font-size:15px;">27 заданий · Python · Пошаговые решения</div>
</div>

## 📋 Навигация по заданиям

| № | Тема | Статус | Ссылка |
|:---:|:---|:---:|:---|
| **1** | Анализ информационных моделей | ✅ | [Перейти →](./Lectures/1/README.md) |
| **2** | Таблицы истинности логических выражений | ✅ | [Перейти →](./Lectures/2/README.md) |
| **3** | Поиск и сортировка в базах данных | 🚧 | — |
| **4** | Кодирование и декодирование данных | 🚧 | — |
| **5** | Анализ алгоритмов для исполнителей | 🚧 | — |
| **6** | Циклические алгоритмы для Исполнителя | ✅ | [Перейти →](./Lectures/6/Razbor-zadaniya-6-iz-EGE-po-informatike.pdf) |
| **7** | Кодирование графической и звуковой информации | 🚧 | — |
| **8** | Комбинаторика | ✅ | [Перейти →](./Lectures/8/README.md) |
| **9** | Обработка числовой информации в электронных таблицах | ✅ | [Перейти →](./Lectures/9/README.md) |
| **10** | Поиск слова в текстовом документе | ✅ | [Перейти →](./Lectures/10/main.ipynb) |
| **11** | Вычисление количества информации | 🚧 | — |
| **12** | Машина Тьюринга | 🚧 | — |
| **13** | IP адреса и маски | 🚧 | — |
| **14** | Позиционные системы счисления | 🚧 | — |
| **15** | Истинность логического выражения | 🚧 | — |
| **16** | Вычисление значения рекурсивной функции | 🚧 | — |
| **17** | Обработка целочисленных данных. Проверка делимости | ✅ | [Перейти →](./Lectures/17/main.ipynb) |
| **18** | Динамическое программирование в электронных таблицах | 🚧 | — |
| **19–21** | Теория игр | 🚧 | — |
| **22** | Многопоточные вычисления | ✅ | [Перейти →](./Lectures/22/README.ipynb) |
| **23** | Динамическое программирование | 🚧 | — |
| **24** | Обработка символьной информации | ✅ | [Перейти →](./Lectures/24/README.ipynb) |
| **25** | Поиск делителей | 🚧 | — |
| **26** | Обработка данных с помощью сортировки | 🚧 | — |
| **27** | Анализ данных | 🚧 | — |

> ✅ — готово · 🚧 — в разработке

## 🚀 Как пользоваться

<div style="display:grid;grid-template-columns:1fr 1fr 1fr;gap:12px;margin:16px 0;">

<div style="background:#0d1b2a;border:1px solid #1b3a5c;border-radius:10px;padding:16px;">
<div style="color:#1b91ff;font-size:20px;margin-bottom:8px;">1️⃣</div>
<div style="color:#ffffff;font-weight:700;margin-bottom:4px;">Выберите задание</div>
<div style="color:#8ab4d4;font-size:13px;">Найдите нужный номер в таблице выше</div>
</div>

<div style="background:#0d1b2a;border:1px solid #1b3a5c;border-radius:10px;padding:16px;">
<div style="color:#e07b39;font-size:20px;margin-bottom:8px;">2️⃣</div>
<div style="color:#ffffff;font-weight:700;margin-bottom:4px;">Откройте лекцию</div>
<div style="color:#8ab4d4;font-size:13px;">Файл <code>.ipynb</code> откроется в Jupyter или Google Colab</div>
</div>

<div style="background:#0d1b2a;border:1px solid #1b3a5c;border-radius:10px;padding:16px;">
<div style="color:#2fca72;font-size:20px;margin-bottom:8px;">3️⃣</div>
<div style="color:#ffffff;font-weight:700;margin-bottom:4px;">Решайте задачи</div>
<div style="color:#8ab4d4;font-size:13px;">Сначала попробуйте сами, потом смотрите разбор</div>
</div>

</div>

## 🔗 Полезные ссылки

- [Открыть курс в Google Colab](https://colab.research.google.com/github/LittleBrotherProg/Lectures/)
- [Скачать все материалы](./archive.zip)
