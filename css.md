# CSS Cheat Sheet

## Основы

### Подключение CSS
- **Inline CSS:**
```html
<h1 style="color: red;">Hello World</h1>
```
- **Internal CSS:**
```html
<style>
h1 { color: red; }
</style>
```
- **External CSS:**
```html
<link rel="stylesheet" href="styles.css">
```

## Селекторы

### Основные селекторы
- **Селектор по тегу:**
```css
p {
color: blue;
}
```
- **Селектор по классу:**
```css
.classname {
font-size: 20px;
}
```
- **Селектор по ID:**
```css
#idname {
background-color: yellow;
}
```
- **Группировка селекторов:**
```css
h1, h2, h3 {
font-family: Arial, sans-serif;
}
```

### Комбинированные селекторы
- **Потомок:**
```css
div p {
margin: 10px;
}
```
- **Дочерний элемент:**
```css
ul > li {
list-style-type: none;
}
```
- **Псевдоклассы:**
```css
a
{
color: red;
}
```

## Основные свойства

### Цвет и фон
- **Цвет текста:**
```css
color: #333;
```
- **Цвет фона:**
```css
background-color: #f0f0f0;
```
- **Фоновое изображение:**
```css
background-image: url('background.jpg');
background-size: cover;
```

### Текст и шрифты
- **Шрифт текста:**
```css
font-family: 'Arial', sans-serif;
```
- **Размер шрифта:**
```css
font-size: 16px;
```
- **Толщина шрифта:**
```css
font-weight: bold;
```
- **Высота строки:**
```css
line-height: 1.5;
```
- **Выравнивание текста:**
```css
text-align: center;
```

### Отступы и границы
- **Внешние отступы (margin):**
```css
margin: 20px;
```
- **Внутренние отступы (padding):**
```css
padding: 10px;
```
- **Граница (border):**
```css
border: 1px solid #ccc;
```
- **Радиус границы:**
```css
border-radius: 5px;
```

### Блочная модель
- **Ширина и высота:**
```css
width: 200px;
height: 100px;
```
- **Максимальная и минимальная ширина:**
```css
max-width: 100%;
min-width: 300px;
```

## Flexbox

### Основные свойства
- **Контейнер:**
```css
display: flex;
justify-content: space-between;
align-items: center;
```
- **Направление flex:**
```css
flex-direction: row;
```
- **Обертка flex:**
```css
flex-wrap: wrap;
```

### Свойства элементов
- **Размер элемента (grow, shrink, basis):**
```css
flex-grow: 1;
flex-shrink: 1;
flex-basis: 100px;
```
- **Выравнивание самого себя:**
```css
align-self: flex-start;
```

## Позиционирование

### Основные типы позиционирования
- **Относительное позиционирование:**
```css
position: relative;
top: 10px;
left: 20px;
```
- **Абсолютное позиционирование:**
```css
position: absolute;
top: 50px;
right: 20px;
```
- **Фиксированное позиционирование:**
```css
position: fixed;
bottom: 0;
right: 0;
```

## Прочее

### Тени
- **Тень блока:**
```css
box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
```
- **Тень текста:**
```css
text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
```

### Переходы и анимации
- **Переход:**
```css
transition: all 0.3s ease;
```
- **Анимация:**
```css
@keyframes example {
from { opacity: 0; }
to { opacity: 1; }
}

.element {
animation: example 2s infinite;
}
```

### Видимость и отображение
- **Скрытие элемента:**
```css
display: none;
```
- **Видимость элемента:**
```css
visibility: hidden;
```

### Z-индекс
- **Управление слоем:**
```css
z-index: 10;
```

## Советы и рекомендации

### Специфичность
- **Порядок применения стилей:**

Inline стили 
самаявысокаяспецифичность
самаявысокаяспецифичность.
Идентификаторы 
#
𝑖
𝑑
#id.
Классы 
𝑐
˙
𝑙
𝑎
𝑠
𝑠
c
˙
 lass и атрибуты.
Теги 
\element
\element.
### Сокращенные записи
- **Отступы:**
```css
padding: 10px 20px 10px 20px; /* top, right, bottom, left */
```
- **Границы:**
```css
border: 1px solid #000; /* width, style, color */
```
