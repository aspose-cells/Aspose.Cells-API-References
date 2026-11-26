---
title: "PivotTable.AltTextDescription"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Получает описание альтернативного текста"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/alttextdescription/
---
## PivotTable.AltTextDescription property

Получает описание альтернативного текста.

```csharp
public string AltTextDescription { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyAltTextDescriptionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте образцовые данные для сводной таблицы
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Создайте сводную таблицу
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Добавьте поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Отобразить текущее описание альтернативного текста
            Console.WriteLine("Current AltTextDescription: " + pivotTable.AltTextDescription);

            // Установить новое описание альтернативного текста
            pivotTable.AltTextDescription = "Sales data by product category";

            // Сохраните книгу
            workbook.Save("PivotTableAltTextDescriptionDemo.xlsx");

            // Отобразить новое описание альтернативного текста
            Console.WriteLine("New AltTextDescription: " + pivotTable.AltTextDescription);
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


