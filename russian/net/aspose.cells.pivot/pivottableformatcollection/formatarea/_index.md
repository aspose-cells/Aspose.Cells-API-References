---
title: "PivotTableFormatCollection.FormatArea"
second_title: "Справочник API Aspose.Cells для .NET"
description: "PivotTableFormatCollection метод. Форматирует выбранную область"
type: docs
url: /ru/net/aspose.cells.pivot/pivottableformatcollection/formatarea/
---
## PivotTableFormatCollection.FormatArea method

Форматирует выбранную область.

```csharp
public PivotTableFormat FormatArea(PivotFieldType axisType, int fieldPosition, 
    PivotFieldSubtotalType subtotalType, PivotTableSelectionType selectionType, bool isGrandRow, 
    bool isGrandColumn, Style style)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| axisType | PivotFieldType | Область PivotTable, к которой применяется это правило. |
| fieldPosition | Int32 | Позиция поля в пределах оси, к которой применяется это правило. |
| subtotalType | PivotFieldSubtotalType | Тип фильтра подытога поля сводной таблицы |
| selectionType | PivotTableSelectionType | Указывает, как выбирать данные. |
| isGrandRow | Boolean | Указывает, выбираются ли строки общей суммы. |
| isGrandColumn | Boolean | Указывает, выбираются ли столбцы общей суммы. |
| стиль | Стиль | Стиль, применяемый к области сводной таблицы. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PivotTableFormatCollectionMethodFormatAreaWithPivotFieldTypeInt32PivotFieldSDemo
    {
        public static void Run()
        {
            // Создайте рабочую книгу из исходного файла
            Workbook workbook = new Workbook("example.xlsx");
            
            // Получить доступ к сводной таблице
            PivotTable pt = workbook.Worksheets["PIVOT_VBA_SUBTOTALS"].PivotTables[0];
            
            // Создать стиль для форматирования
            Style style = workbook.CreateStyle();
            style.SetBorder(BorderType.LeftBorder, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.RightBorder, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.TopBorder, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, Color.Red);
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = Color.LightGray;
            style.BackgroundColor = Color.LightGray;

            // Форматировать область сводной таблицы
            pt.PivotFormats.FormatArea(
                PivotFieldType.Row, 
                0, 
                PivotFieldSubtotalType.Automatic, 
                PivotTableSelectionType.DataAndLabel, 
                false, 
                false, 
                style);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [PivotTableFormat](../../pivottableformat/)
* enum [PivotFieldType](../../pivotfieldtype/)
* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* enum [PivotTableSelectionType](../../pivottableselectiontype/)
* class [Style](../../../aspose.cells/style/)
* class [PivotTableFormatCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


