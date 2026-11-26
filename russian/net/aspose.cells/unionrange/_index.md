---
title: "Класс UnionRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.UnionRange. Представляет объединённый диапазон"
type: docs
url: /ru/net/aspose.cells/unionrange/
---
## UnionRange class

Представляет объединённый диапазон.

```csharp
public class UnionRange : IEnumerable
```

## Свойства

| Имя | Описание |
| --- | --- |
| [CellCount](../../aspose.cells/unionrange/cellcount/) { get; } | Получает общее количество ячеек в диапазоне. |
| [ColumnCount](../../aspose.cells/unionrange/columncount/) { get; } | Получает количество строк в диапазоне. |
| [FirstColumn](../../aspose.cells/unionrange/firstcolumn/) { get; } | Получает индекс первого столбца диапазона. |
| [FirstRow](../../aspose.cells/unionrange/firstrow/) { get; } | Получает индекс первой строки диапазона. |
| [HasRange](../../aspose.cells/unionrange/hasrange/) { get; } | Указывает, имеет ли это диапазон. |
| [Hyperlinks](../../aspose.cells/unionrange/hyperlinks/) { get; } | Получает все гиперссылки в диапазоне. |
| [Name](../../aspose.cells/unionrange/name/) { get; set; } | Получает или задает имя диапазона. |
| [RangeCount](../../aspose.cells/unionrange/rangecount/) { get; } | Получает количество диапазонов. |
| [Ranges](../../aspose.cells/unionrange/ranges/) { get; } | Получает все объединённые диапазоны. |
| [RefersTo](../../aspose.cells/unionrange/refersto/) { get; } | Получает значение свойства RefersTo диапазона. |
| [RowCount](../../aspose.cells/unionrange/rowcount/) { get; } | Получает количество строк в диапазоне. |
| [Value](../../aspose.cells/unionrange/value/) { get; set; } | Получает и задаёт значения диапазона. |

## Методы

| Имя | Описание |
| --- | --- |
| [ApplyStyle](../../aspose.cells/unionrange/applystyle/)(Style, StyleFlag) | Применяет форматы ко всему диапазону. |
| [Copy](../../aspose.cells/unionrange/copy/)(UnionRange, PasteOptions) | Копирует диапазон с параметрами специальной вставки. |
| [GetEnumerator](../../aspose.cells/unionrange/getenumerator/)() | Получает перечислитель для ячеек в этом Range. |
| [Intersect](../../aspose.cells/unionrange/intersect/#intersect)(Range[]) | Пересекает другой диапазон. |
| [Intersect](../../aspose.cells/unionrange/intersect/#intersect_2)(string) | Пересекает другой диапазон. |
| [Intersect](../../aspose.cells/unionrange/intersect/#intersect_1)(UnionRange) | Пересекает другой диапазон. |
| [Merge](../../aspose.cells/unionrange/merge/)() | Объединяет диапазон ячеек в одну ячейку. |
| [PutValue](../../aspose.cells/unionrange/putvalue/)(string, bool, bool) | Помещает значение в диапазон; при необходимости значение будет преобразовано в другой тип данных, а числовой формат ячейки будет сброшен. |
| [SetOutlineBorders](../../aspose.cells/unionrange/setoutlineborders/#setoutlineborders)(CellBorderType, Color) | Устанавливает контурные границы вокруг диапазона ячеек с одинаковым стилем и цветом границы. |
| [SetOutlineBorders](../../aspose.cells/unionrange/setoutlineborders/#setoutlineborders_1)(CellBorderType[], Color[]) | Устанавливает внешние границы вокруг диапазона ячеек. |
| [SetStyle](../../aspose.cells/unionrange/setstyle/)(Style) | Устанавливает стиль диапазона. |
| [Union](../../aspose.cells/unionrange/union/#union)(Range[]) | Объединить диапазоны. |
| [Union](../../aspose.cells/unionrange/union/#union_2)(string) | Объединить другой диапазон. |
| [Union](../../aspose.cells/unionrange/union/#union_1)(UnionRange) | Объединить другой диапазон. |
| [UnMerge](../../aspose.cells/unionrange/unmerge/)() | Разъединяет объединённые ячейки этого диапазона. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassUnionRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создайте объединённый диапазон, используя правильный API
            UnionRange unionRange = workbook.Worksheets.CreateUnionRange("A1:A10,C1:C10", 0);
            
            // Установить значение для всего объединённого диапазона
            unionRange.Value = "Test";
            
            // Применить стиль к объединённому диапазону
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            unionRange.ApplyStyle(style, new StyleFlag { All = true });
            
            // Сохраните книгу
            workbook.Save("UnionRangeDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


