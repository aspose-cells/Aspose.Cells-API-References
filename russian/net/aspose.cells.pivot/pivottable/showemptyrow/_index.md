---
title: "PivotTable.ShowEmptyRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Указывает, включать ли пустые строки в таблицу"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/showemptyrow/
---
## PivotTable.ShowEmptyRow property

Указывает, включать ли пустые строки в таблицу.

```csharp
public bool ShowEmptyRow { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyShowEmptyRowDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные с некоторыми пустыми строками
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["B1"].Value = "Product";
            worksheet.Cells["C1"].Value = "Sales";
            
            worksheet.Cells["A2"].Value = "Electronics";
            worksheet.Cells["B2"].Value = "TV";
            worksheet.Cells["C2"].Value = 1000;
            
            worksheet.Cells["A3"].Value = "Electronics";
            worksheet.Cells["B3"].Value = "";
            worksheet.Cells["C3"].Value = "";
            
            worksheet.Cells["A4"].Value = "Furniture";
            worksheet.Cells["B4"].Value = "Chair";
            worksheet.Cells["C4"].Value = 500;
            
            worksheet.Cells["A5"].Value = "Furniture";
            worksheet.Cells["B5"].Value = "";
            worksheet.Cells["C5"].Value = "";

            // Создайте сводную таблицу
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Добавьте поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Отобразить текущее значение ShowEmptyRow
            Console.WriteLine("Initial ShowEmptyRow value: " + pivotTable.ShowEmptyRow);

            // Показать пустые строки в сводной таблице
            pivotTable.ShowEmptyRow = true;
            Console.WriteLine("ShowEmptyRow set to: " + pivotTable.ShowEmptyRow);

            // Вычислить данные для заполнения сводной таблицы
            pivotTable.CalculateData();

            // Сохраните книгу
            workbook.Save("PivotTableShowEmptyRowDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


