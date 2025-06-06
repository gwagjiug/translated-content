---
title: shape-rendering
slug: Web/SVG/Reference/Attribute/shape-rendering
---

{{SVGRef}}

« [Справочник SVG атрибутов](/ru/docs/Web/SVG/Reference/Attribute)

При создании SVG есть возможность указать браузеру, как рекомендуется рендерить (отрисовывать) элементы {{ SVGElement("path") }} или базовые фигуры. `shape-rendering` предоставляет возможность указывать данные рекомендации.

## Контекст использования

| Категория            | Атрибут представления                                                                     |
| -------------------- | ----------------------------------------------------------------------------------------- |
| Значения             | **auto** \| optimizeSpeed \| crispEdges \| geometricPrecision \| inherit                  |
| Анимация             | Да                                                                                        |
| Нормативный документ | [SVG 1.1 (2nd Edition)](https://www.w3.org/TR/SVG11/painting.html#ShapeRenderingProperty) |

- auto
  - : Указывает на то, что браузер должен внести соответствующие компромиссы, чтобы сбалансировать скорость рендеринга, чёткие края и геометрическую точность, но геометрической точности уделять более пристальное внимание, чем скорости и чётким краями.
- optimizeSpeed
  - : Указывает на то, что браузер должен акцентироваться на скорость рендеринга, в ущерб геометрической точности и чётким краями. Эту опцию также можно указывать,, чтобы отключить сглаживание фигур.
- crispEdges
  - : Указывает на то, что браузер должен попытаться акцентировать на контрасте чистых краёв рисунков, в ущерб скорости рендеринга и геометрической точности. Для достижения наилучшего результата чёткости края, браузер может отключить сглаживание для всех линий и кривых или, возможно, только для прямых, близких к вертикальным или горизонтальным. Кроме того, браузер может скорректировать позиции строк и ширину линий для выравнивания краёв с пикселями устройства.
- geometricPrecision
  - : Указывает на то, что браузер должен акцентировать геометрическую точность в ущерб скорости и чёткими краям.

## Пример

```xml
<svg xmlns="http://www.w3.org/2000/svg"
  version="1.1" width="100" height="100"
  shape-rendering="optimizeSpeed">
```

| shape-rendering: geometricPrecision:![shape-rendering:geometricPrecision](http://download.g63.ru/svg/shape-rendering-geometricPrecision.svg) | shape-rendering: optimizeSpeed![shape-rendering:optimizeSpeed](http://download.g63.ru/svg/shape-rendering-optimizeSpeed.svg) |
| -------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- |

Также можно воспользоваться css shape-rendering:

```xml
<svg xmlns="http://www.w3.org/2000/svg"
  version="1.1" width="100" height="100"
  style="shape-rendering:optimizeSpeed;">
```

## Элементы

Следующие элементы могут использовать атрибут `shape-rendering`

- [Shape elements](/en-US/SVG/Element#shape)
