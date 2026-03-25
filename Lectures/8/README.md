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
<div style="background:linear-gradient(135deg,#1a2332 0%,#0d1b2a 100%);border-radius:16px;padding:36px;margin-bottom:12px;">
  <div style="display:flex;align-items:center;gap:18px;margin-bottom:16px;">
    <div style="background:#1b91ff;color:#fff;font-size:36px;font-weight:900;border-radius:12px;padding:8px 20px;">8</div>
    <div>
      <div style="color:#8ab4d4;font-size:12px;font-weight:600;letter-spacing:3px;text-transform:uppercase;">ЕГЭ по информатике</div>
      <div style="color:#ffffff;font-size:24px;font-weight:800;">Комбинаторика</div>
      
    </div>
  </div>
  <div style="display:flex;gap:8px;flex-wrap:wrap;"><span style="background:#1b3a5c;color:#7ec8e3;font-size:12px;padding:4px 14px;border-radius:20px;font-weight:600;">Python</span> <span style="background:#1b3a5c;color:#7ec8e3;font-size:12px;padding:4px 14px;border-radius:20px;font-weight:600;">Перебор</span> <span style="background:#1b3a5c;color:#7ec8e3;font-size:12px;padding:4px 14px;border-radius:20px;font-weight:600;">Комбинации</span> </div>
</div>

<div style="background:#0a1628;border:1px solid #1b3a5c;border-radius:8px;padding:10px 18px;margin-bottom:16px;display:inline-block;">
<a href="../../README.md" style="color:#1b91ff;text-decoration:none;font-weight:600;">← Назад ко всем заданиям</a>
</div>


## 🔙 Навигация
[← Назад к списку всех заданий](../README.md)

## 📖 Лекции по заданию 8

### 1. Задачи с цифрами
*   [**Лекция 1:** Количество чисел с ограничениями](./Tasks_numbers/task_8_combinatorics.ipynb)
    *   [Открыть в Colab](https://colab.research.google.com/github/ВАШ_ЛОГИН/НАЗВАНИЕ_РЕПОЗИТОРИЯ/blob/main/task_08/lecture_1_digital.ipynb)
*   [**Лекция 2:** Четность и чередование цифр](./Tasks_numbers/task_8.1_combinatorics.ipynb)
    *   [Открыть в Colab](https://colab.research.google.com/github/ВАШ_ЛОГИН/НАЗВАНИЕ_РЕПОЗИТОРИЯ/blob/main/task_08/lecture_2_parity.ipynb)

### 2. Задачи с буквами  
*   [**Лекция 3:** Поиск номера комбинации](./Tasks_letters/task_8.2.ipynb)
    *   [Открыть в Colab](https://colab.research.google.com/github/ВАШ_ЛОГИН/НАЗВАНИЕ_РЕПОЗИТОРИЯ/blob/main/task_08/lecture_3_letters.ipynb)

## 🎯 Типовые случаи в задании 8

*   Подсчет количества чисел в различных системах счисления
*   Составление слов по заданным правилам
*   Работа с ограничениями на повторения и соседство символов
*   Поиск номера комбинации в упорядоченном списке