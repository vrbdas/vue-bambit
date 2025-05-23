# Галерея фото — тестовое задание frontend-разработчика

Приложение загружает фотографии с публичного API jsonplaceholder и отображает их в таблице с динамической подгрузкой и сортировкой по столбцам. Реализован фильтр по ID альбомов с поддержкой множественного ввода. При пустом фильтре загружаются все фотографии.

Реализованы тёмная и светлая темы с сохранением выбранной темы и фильтров в `localStorage`. Шапка таблицы прилипает при прокрутке.

**Используемые технологии:**  
- Vue 3 (Composition API, `<script setup>`)  
- Pinia для управления состоянием и кеширования данных  
- Tailwind CSS для стилизации  
- Axios для работы с API

**Особенности:**  
- Автоматическая загрузка фотографий при старте  
- Пагинация и ленивая подгрузка при скролле  
- Сортировка по всем данным с обратным порядком при повторном клике  
- Подсказки (tooltip) при обрезанном тексте в ячейках  
- Спиннер загрузки  
- Фильтрация по нескольким альбомам с поддержкой запросов с несколькими параметрами `albumId`

[Демо проекта](https://devartmax.ru/photoscope/)

_Примечание:_ API jsonplaceholder -  бесплатный сервис с "cold start" (холодным стартом), поэтому первая загрузка таблицы может занять 30–50 секунд.
