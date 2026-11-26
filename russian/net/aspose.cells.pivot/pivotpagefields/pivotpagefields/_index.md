---
title: "PivotPageFields.PivotPageFields"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор PivotPageFields. Представляет элементы поля страницы сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivotpagefields/pivotpagefields/
---
## PivotPageFields constructor

Представляет элементы полей страниц сводной таблицы.

```csharp
public PivotPageFields()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotPageFieldsMethodSharpctorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue("East");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue("West");
            worksheet.Cells["C3"].PutValue(2000);

            // Создайте поля страницы сводной таблицы с помощью конструктора
            PivotPageFields pageFields = new PivotPageFields();
            
            // Добавить поля страницы
            string[] items = { "Item1", "Item2" };
            pageFields.AddPageField(items);
            
            // Добавить идентификацию
            int[] itemIndexes = { 0, 1 };
            pageFields.AddIdentify(0, itemIndexes);

            // Добавить сводную таблицу с правильными параметрами
            PivotTableCollection pivotTables = worksheet.PivotTables;
            string sourceData = "A1:C3";
            int index = pivotTables.Add(sourceData, "E5", "PivotTable1");

            // Сохраните книгу
            workbook.Save("PivotPageFieldsDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotPageFields](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


