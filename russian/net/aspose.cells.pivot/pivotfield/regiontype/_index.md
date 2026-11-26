---
title: "PivotField.RegionType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotField. Указывает область сводной таблицы, в которой отображается это поле"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/regiontype/
---
## PivotField.RegionType property

Указывает область сводной таблицы, в которой отображается это поле.

```csharp
public PivotFieldType RegionType { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldPropertyRegionTypeDemo
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
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Добавить поле строки
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Добавить поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Обновить данные сводной таблицы
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Получить первое поле сводной таблицы
            PivotField pivotField = pivotTable.RowFields[0];

            // Отобразить текущее значение RegionType
            Console.WriteLine("Current RegionType value: " + pivotField.RegionType);

            // Продемонстрировать, как использовать свойство RegionType
            if (pivotField.RegionType == PivotFieldType.Row)
            {
                Console.WriteLine("This pivot field is in the row area");
            }

            // Сохраните книгу
            workbook.Save("PivotFieldRegionTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


