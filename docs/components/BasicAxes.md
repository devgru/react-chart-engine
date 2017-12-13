# BasicAxes

Компонент отрисовывает стандартные оси с сеткой, используемые в графиках.

Компонент рендерит `g`-элемент.

Компонент использует компоненты-оси из пакета `react-d3-components`, аналогичные осям создаваемым библиотекой `d3`.

Настроенные шкалы используются для вычисления положения и размеров осей, размещения подписей и создания псевдосетки из их засечек.

## Свойства

Компонент не принимает вложенных элементов.

Все свойства **обязательны**.

- [шкала](https://github.com/d3/d3-scale#continuous-scales) `xScale` для оси абсцисс;
- [шкала](https://github.com/d3/d3-scale#continuous-scales) `yScale` для оси ординат;
- число `xPadding`, горизонтальный отступ от оси до текста для оси ординат;
- число `yPadding`, вертикальный отступ от оси до текста для оси абсцисс;
- число `width`, ширина «рабочей» зоны графика;
- число `height`, высота «рабочей» зоны графика.

Шкалы могут быть созданы с помощью `d3` версий 3 и 4.