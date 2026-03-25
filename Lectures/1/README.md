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
    <div style="background:#1b91ff;color:#fff;font-size:36px;font-weight:900;border-radius:12px;padding:8px 20px;">1</div>
    <div>
      <div style="color:#8ab4d4;font-size:12px;font-weight:600;letter-spacing:3px;text-transform:uppercase;">ЕГЭ по информатике</div>
      <div style="color:#ffffff;font-size:24px;font-weight:800;">Анализ информационных моделей</div>
      
    </div>
  </div>
  <div style="display:flex;gap:8px;flex-wrap:wrap;"><span style="background:#1b3a5c;color:#7ec8e3;font-size:12px;padding:4px 14px;border-radius:20px;font-weight:600;">Граф</span> <span style="background:#1b3a5c;color:#7ec8e3;font-size:12px;padding:4px 14px;border-radius:20px;font-weight:600;">Таблица</span> <span style="background:#1b3a5c;color:#7ec8e3;font-size:12px;padding:4px 14px;border-radius:20px;font-weight:600;">Кратчайший путь</span> </div>
</div>

<div style="background:#0a1628;border:1px solid #1b3a5c;border-radius:8px;padding:10px 18px;margin-bottom:16px;display:inline-block;">
<a href="../../README.md" style="color:#1b91ff;text-decoration:none;font-weight:600;">← Назад ко всем заданиям</a>
</div>


Задание №1 ЕГЭ по информатике проверяет умение анализировать простые информационные модели, представленные в виде таблиц (матриц смежности) и графов (схем дорог). Часто требуется найти кратчайший путь между двумя точками или установить соответствие между номерами в таблице и буквами на схеме.

**Основные типы задач:**
- Найти сумму протяжённостей дорог между двумя точками.  
- Установить соответствие между номерами в таблице и буквами на схеме.  
- Найти количество возможных маршрутов или определить наличие/отсутствие пути.

## 🔍 Теория: Что такое информационная модель?

Информационная модель — это способ представления реального объекта или процесса с помощью данных и их связей.

В контексте задания №1:
- **Таблица** — матрица смежности, где строки и столбцы — это населённые пункты, а ячейки — расстояния между ними (или звёздочка `*`, если дороги нет).
- **Граф** — схема, где вершины — населённые пункты, а рёбра — дороги между ними.

> **Важно:** Таблица и схема составлены независимо друг от друга. Нумерация в таблице **не связана** с буквами на схеме. Это ключевой момент!
## 🧩 Пример решения задачи №1

### Условие задачи

На рисунке схема дорог Н-ского района изображена в виде графа, а в таблице приведены длины этих дорог (в километрах).

![Схема и таблица](img/one.png)

> **Важно!** Таблицу и схему составляли независимо друг от друга. Это значит, что пункты в таблице (П1, П2, П3...) никак не связаны с буквами на схеме (А, Б, В...). Наша задача — установить соответствие между ними.

**Вопрос:** Чему равна протяжённость дороги из пункта **К** в пункт **Г**? Ответ запишите целым числом.

---

### 🔍 Шаг 1. Анализ таблицы

Сначала посмотрим на таблицу и определим, сколько дорог выходит из каждого пункта (то есть сколько чисел стоит в каждой строке):

- **П1**: соединён с П2 и П4 → **2 дороги**  
- **П2**: соединён с П1, П4, П6 → **3 дороги**  
- **П3**: соединён с П5 и П6 → **2 дороги**  
- **П4**: соединён с П1, П2, П6, П7 → **4 дороги**  
- **П5**: соединён с П3 и П6 → **2 дороги**  
- **П6**: соединён с П2, П3, П4, П5, П7 → **5 дорог**  
- **П7**: соединён с П4 и П6 → **2 дороги**

![Анализ таблицы](img/g2.gif)

---

### 🔍 Шаг 2. Анализ схемы

Теперь посмотрим на граф и посчитаем, сколько рёбер (дорог) выходит из каждой вершины:

- У **В** — 5 дорог → это уникальный пункт!  
- У **Е** — 4 дороги  
- У **Г** — 3 дороги  
- У **А, Б, Д, К** — по 2 дороги

![Пункт с 5 дорогами](img/g3.gif)

Поскольку **только один** пункт в таблице имеет 5 дорог — это **П6**, а на схеме — только **В**, значит:

> **В ↔ П6**

---

### 🔍 Шаг 3. Определяем пункты А и Б

Пункты **А** и **Б** соединены только между собой и с пунктом **В** (П6). У каждого из них — по 2 дороги.

В таблице ищем два пункта, которые:
- соединены между собой,
- соединены с **П6**,
- и больше ни с кем не соединены.

Это **П3** и **П5**.

> **А и Б ↔ П3 и П5** (точное соответствие пока не важно).

![А и Б](img/g4.gif)

---

### 🔍 Шаг 4. Находим пункт Е

На схеме у пункта **Е** — 4 дороги. В таблице такой пункт тоже один — **П4**.

> **Е ↔ П4**

![Пункт Е](img/g5.gif)

---

### 🔍 Шаг 5. Определяем пункт Д

Пункт **Д** соединён только с **Е** и **В** (то есть с П4 и П6). У него 2 дороги.

В таблице такой пункт — **П7**.

> **Д ↔ П7**

![Пункт Д](img/g6.gif)

---

### 🔍 Шаг 6. Определяем К и Г

Остались неопознанными:
- На схеме: **К** (2 дороги), **Г** (3 дороги)  
- В таблице: **П1** (2 дороги), **П2** (3 дороги)

Сопоставляем:
- **К ↔ П1**  
- **Г ↔ П2**

![К и Г](img/g7.gif)

---

### ✅ Шаг 7. Находим ответ

Нас просят найти длину дороги **из К в Г** → это **из П1 в П2**.

Смотрим в таблицу: на пересечении **П1** и **П2** стоит число **45**.

![Ответ](img/g8.gif)

> **Ответ: 45**