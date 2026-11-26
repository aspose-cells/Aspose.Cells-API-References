---
title: "PivotTable.SourceType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Получает тип источника данных сводной таблицы."
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/sourcetype/
---
## PivotTable.SourceType property

Получает тип источника данных сводной таблицы.

```csharp
public PivotTableSourceType SourceType { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertySourceTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте образцовые данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Region";
            worksheet.Cells["C1"].Value = "Sales";
            
            worksheet.Cells["A2"].Value = "Product A";
            worksheet.Cells["B2"].Value = "North";
            worksheet.Cells["C2"].Value = 1000;
            
            worksheet.Cells["A3"].Value = "Product B";
            worksheet.Cells["B3"].Value = "South";
            worksheet.Cells["C3"].Value = 2000;
            
            worksheet.Cells["A4"].Value = "Product C";
            worksheet.Cells["B4"].Value = "East";
            worksheet.Cells["C4"].Value = 3000;

            // Создайте сводную таблицу
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("=A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Добавьте поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Отобразить текущее значение SourceType.
            Console.WriteLine("Current PivotTable SourceType: " + pivotTable.SourceType);

            // Вычислить данные для отображения сводной таблицы.
            pivotTable.CalculateData();

            // Сохраните книгу
            workbook.Save("PivotTableSourceTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [PivotTableSourceType](../../pivottablesourcetype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


