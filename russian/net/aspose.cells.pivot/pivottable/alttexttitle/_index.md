---
title: "PivotTable.AltTextTitle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Получает и задает заголовок альтернативного текста"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/alttexttitle/
---
## PivotTable.AltTextTitle property

Получает и задает заголовок изменённого текста.

```csharp
public string AltTextTitle { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyAltTextTitleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте образцовые данные для сводной таблицы
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["B2"].PutValue("North");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B3"].PutValue("South");
            worksheet.Cells["C3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Product C");
            worksheet.Cells["B4"].PutValue("East");
            worksheet.Cells["C4"].PutValue(3000);

            // Создайте сводную таблицу
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:C4", "E3", "SalesPivotTable");
            PivotTable pivotTable = pivotTables[index];

            // Добавьте поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Отобразить текущее значение AltTextTitle
            Console.WriteLine("Current AltTextTitle value: " + pivotTable.AltTextTitle);

            // Установить новое значение AltTextTitle
            pivotTable.AltTextTitle = "Sales Data Pivot Table";

            // Вычислить данные сводной таблицы
            pivotTable.CalculateData();

            // Сохраните книгу
            workbook.Save("PivotTableAltTextTitleDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


