---
title: "PivotTableFormat.PivotArea"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTableFormat. Возвращает область сводки"
type: docs
url: /ru/net/aspose.cells.pivot/pivottableformat/pivotarea/
---
## PivotTableFormat.PivotArea property

Получает область сводной таблицы.

```csharp
public PivotArea PivotArea { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableFormatPropertyPivotAreaDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["A3"].PutValue("Vegetable");
            sheet.Cells["B1"].PutValue("Amount");
            sheet.Cells["B2"].PutValue(50);
            sheet.Cells["B3"].PutValue(30);

            // Создать сводную таблицу
            int pivotIndex = sheet.PivotTables.Add("A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // Добавить поля в области сводной таблицы
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Получите формат сводки и настройте его область
            int formatIndex = pivotTable.PivotFormats.Add();
            PivotTableFormat pivotFormat = pivotTable.PivotFormats[formatIndex];
            PivotArea pivotArea = pivotFormat.PivotArea;
            
            // Установите свойства области сводки
            pivotArea.AxisType = PivotFieldType.Data;
            pivotArea.IsRowGrandIncluded = true;
            pivotArea.IsColumnGrandIncluded = true;

            // Создайте и примените стиль к области сводки
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            pivotFormat.SetStyle(style);

            // Сохраните книгу
            workbook.Save("PivotTableWithPivotArea.xlsx");
        }
    }
}
```

### См. также

* class [PivotArea](../../pivotarea/)
* class [PivotTableFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


