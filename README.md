# Menu_underline
Це меню створене з навчальною ціллю для учнів WebStudio_PDM. Тема створення меню, використання псевдокласів, різне підкреслення посилань.

## [Demo on Codepen](https://codepen.io/natalka-litkovets/pen/pobbZPe)

![скан-завдання](https://github.com/user-attachments/assets/e576868c-ff95-4be3-9156-c1ad3ea862df)
## 1. Базові стилі для всієї сторінки
### body {
   font-family: sans-serif;
   font-weight: 300;
   font-size: 24px;
}
### font-family: sans-serif;
- Встановлює шрифт без засічок для всього документа (наприклад Arial, Helvetica).
### font-weight: 300;
- Легкий (тонкий) шрифт.
### font-size: 24px;
- Досить великий розмір тексту — зручно для демонстрацій і навчання.
  
## 2. Контейнер для посилань
.links {
   margin: 0 auto;
   width: 50%;
}
### width: 50%;
- Контейнер займає половину ширини сторінки.
### margin: 0 auto;
- Автоматичні лівий і правий відступи → блок вирівнюється по центру сторінки.

## 3. Загальні стилі для посилань
### a {

text-decoration: none;

position: relative;

}
### text-decoration: none;
- Забирає стандартне підкреслення у посилань.

### position: relative;
- Дуже важливо: робить <a> опорним елементом для псевдоелемента ::before, який має position: absolute.

## 4. Анімація для блоку .left
### Створення псевдоелементу :before
Псевдоелемент ::before створюється лише тоді, коли для нього задано властивість:
content: "";

Це базове правило, яке: 
- створює псевдоелемент,
- описує його вигляд і поведінку.
 ### .left a::before {
   content: "";
   bottom: 0;
   right: 0;
   position: absolute;
   width: 0%;
   height: 20px;
   background-color: #7a0909;
   transition: 0.2s;
   opacity: 0.4;
}

