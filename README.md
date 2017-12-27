Данный проект был создан с использованием:

HTML
CSS
node.js
Socket.io


Используемыме функции:

socket.on("draw_line") lines, c, w, imageCanvasData |Посылаем массив линий. Используем для инструмента "Кисть".
socket.on("draw_straight")point1, point2, c, w, imageCanvasData |Посылаем две точки для инструмента "Линия",где point1 начало сегмента, а point2 - конец.
socket.on("draw_rect")point1, point2, c, w, imageCanvasData |Посылаем две точки для инструмента "Прямоугольник". point1 и point2 являются верхней левой и нижней правой точками прямоугольника. 
socket.on("draw_circle")point1, radius, c, w, imageCanvasData | Посылаем две точки для инструмента "круг". point1 - центр, radius - радиус.
socket.on("eraser")lines, w, imageCanvasData | Посылаем массив линий. Используем для инструмента "Ластик". Начальные и конечные точки используются для функции clearRect(). С ее помощью стираем канвас.
socket.on("request_for_image_data") imageCanvasData | Посылаем актуальную картинку клиентам.|

c - цвет.  
w - размер.  
imageCanvasData - актуальная картинка.

Разработка
Костюхин Дмитрий
