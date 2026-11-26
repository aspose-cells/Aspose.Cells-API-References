---
title: "Класс Style"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.GridDesktop.Style класс. Представляет стиль отображения Excel‑документов, таких как цвет шрифта, выравнивание, границы и т.д."
type: docs
url: /ru/net/aspose.cells.griddesktop/style/
---
## Style class

Представляет стиль отображения Excel‑документа, такой как шрифт, цвет, выравнивание, граница и т.д.

```csharp
public class Style
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [Style](style/)(GridDesktop) | Создайте новый Style для элемента управления |

## Свойства

| Имя | Описание |
| --- | --- |
| [BackgroundColor](../../aspose.cells.griddesktop/style/backgroundcolor/) { get; set; } | Получает или задает цвет фона ячейки; если шаблон стиля не установлен в solid, то он будет применён. |
| [CellLocked](../../aspose.cells.griddesktop/style/celllocked/) { get; set; } | Получает или задает значение, указывающее, можно ли изменять ячейку. |
| [Color](../../aspose.cells.griddesktop/style/color/) { get; set; } | Получает или задает цвет затенения ячейки. Когда шаблон равен none, возвращается Color.Empty; когда шаблон BackgroundType.Solid, возвращается ForegroundColor; в остальных случаях возвращается BackgroundColor. |
| [Custom](../../aspose.cells.griddesktop/style/custom/) { get; set; } | Представляет строку пользовательского числового формата этого объекта стиля. Если пользовательский числовой формат не задан (например, числовой формат встроенный), будет возвращена пустая строка "". |
| [Font](../../aspose.cells.griddesktop/style/font/) { get; set; } | Получает объект [`GridFont`](../../aspose.cells.griddesktop.data/gridfont/). |
| [ForegroundColor](../../aspose.cells.griddesktop/style/foregroundcolor/) { get; set; } | Получает или задает цвет переднего плана стиля. |
| [HAlignment](../../aspose.cells.griddesktop/style/halignment/) { get; set; } | Получает или задает атрибут горизонтального выравнивания. |
| [Indent](../../aspose.cells.griddesktop/style/indent/) { get; set; } | Представляет уровень m_IndentLevel для ячейки или диапазона. Может быть только целым числом от 0 до 15. |
| [NumberType](../../aspose.cells.griddesktop/style/numbertype/) { get; set; } | Получает или задает формат отображения чисел и дат. Шаблоны форматирования различаются для разных регионов. |
| [Pattern](../../aspose.cells.griddesktop/style/pattern/) { get; set; } | Получает или задает тип фонового узора ячейки. |
| [Rotation](../../aspose.cells.griddesktop/style/rotation/) { get; set; } | Представляет угол поворота текста. |
| [Shrink](../../aspose.cells.griddesktop/style/shrink/) { get; set; } | Представляет, автоматически ли текст уменьшается, чтобы поместиться в доступную ширину столбца. |
| [TextDirection](../../aspose.cells.griddesktop/style/textdirection/) { get; set; } | Получает или задает атрибут направления текста. |
| [TextWrapped](../../aspose.cells.griddesktop/style/textwrapped/) { get; set; } | Получает или задает значение, указывающее, переносится ли текст внутри ячейки. |
| [VAlignment](../../aspose.cells.griddesktop/style/valignment/) { get; set; } | Получает или задает атрибут вертикального выравнивания. |

## Методы

| Имя | Описание |
| --- | --- |
| [Clone](../../aspose.cells.griddesktop/style/clone/)() | Создаёт и возвращает копию этого объекта. **NOTE:** Если вы клонируете именованный стиль, имя не копируется, потому что имя стиля должно быть уникальным. Поэтому клонированный стиль не будет "равен" оригинальному стилю. |
| [SetBorderColor](../../aspose.cells.griddesktop/style/setbordercolor/)(BorderType, Color) | Устанавливает цвет указанной границы. |
| [SetBorderLine](../../aspose.cells.griddesktop/style/setborderline/)(BorderType, BorderLineType) | Устанавливает тип линии указанной границы. |

### См. также

* namespace [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../)


