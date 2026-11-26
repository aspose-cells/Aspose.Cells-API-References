---
title: "PivotAreaFilter.Selected"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotAreaFilter. Указывает, имеет ли это поле выделение. Работает только когда PivotTable находится в режиме Outline view"
type: docs
url: /ru/net/aspose.cells.pivot/pivotareafilter/selected/
---
## PivotAreaFilter.Selected property

Указывает, имеет ли это поле выделение. Работает только когда PivotTable находится в режиме Outline.

```csharp
public bool Selected { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotAreaFilterPropertySelectedDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // Создайте сводную таблицу
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Получить фильтр области сводной таблицы
            PivotArea pivotArea = new PivotArea(pivotTable);
            PivotAreaFilter filter = pivotArea.Filters[0];

            // Отобразить текущее значение Selected
            Console.WriteLine("Current Selected value: " + filter.Selected);

            // Изменить значение Selected (влияет только на режим Outline view)
            filter.Selected = true;
            Console.WriteLine("New Selected value: " + filter.Selected);

            // Сохраните книгу
            workbook.Save("PivotAreaFilterSelectedDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotAreaFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


