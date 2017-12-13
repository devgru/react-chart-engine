# ZoomableChart

График с возможностью зума.

Создаёт `svg`-элемент с осями, границами, сеткой и отступами.

В качестве потомка принимает функцию, генератор элементов графика. Функция имеет сигнатуру `generateChart({id, xScale, yScale, width, height})` и должна возвращать элемент для отрисовки или объект с полями `{chart, back, front}`, каждое из которых может содержать элемент для отрисовки.

[Пример использования](../../lib/examples/ZoomDemoChart.jsx) компонента.

## Свойства

Свойства `limits`, `zoomState`, `maxScaleFactor`, `onZoomStateChange` передаются в компонент `ZoomableG` без изменений и имеют значение по умолчанию `undefined`. Про эти свойства см. [ZoomableG](../ZoomableG.md).

- строка `id`, используется для создания идентификаторов некоторых элементов внутри графика, по умолчанию — случайная строка;
- массив из двух чисел `xDomain`, диапазон значений данных по оси абсцисс;
- массив из двух чисел `yDomain`, диапазон значений данных по оси ординат;
- число `xPadding`, горизонтальный отступ от оси до текста для оси ординат;
- число `yPadding`, вертикальный отступ от оси до текста для оси абсцисс;
- объект `margin`, с числовыми полями `left`, `top`, `right` и `bottom`, отступы графика.