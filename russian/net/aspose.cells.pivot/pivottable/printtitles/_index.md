---
title: "PivotTable.PrintTitles"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Указывает, установлены ли заголовки печати для листа на основе отчёта PivotTable. Значение по умолчанию — false"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/printtitles/
---
## PivotTable.PrintTitles property

Указывает, устанавливаются ли заголовки печати для листа на основе отчёта PivotTable. Значение по умолчанию — false.

```csharp
public bool PrintTitles { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPrintTitlesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте лист и некоторые примерные данные
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(300);

            // Создайте сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Настроить поля сводной таблицы
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Продемонстрировать свойство PrintTitles
            pivotTable.PrintTitles = true;
            Console.WriteLine("PrintTitles set to: " + pivotTable.PrintTitles);

            // Сохраните книгу
            workbook.Save("PivotTablePrintTitlesDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


