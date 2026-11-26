---
title: "PivotTable.ShowMemberPropertyTips"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Указывает логическое значение, определяющее, следует ли исключать информацию о свойствах участников из подсказок PivotTable"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/showmemberpropertytips/
---
## PivotTable.ShowMemberPropertyTips property

Задаёт логическое значение, указывающее, следует ли опустить информацию о свойствах членов из подсказок PivotTable.

```csharp
public bool ShowMemberPropertyTips { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyShowMemberPropertyTipsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте образцовые данные для сводной таблицы
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Bike");
            worksheet.Cells["A3"].PutValue("Car");
            worksheet.Cells["A4"].PutValue("Bike");
            worksheet.Cells["A5"].PutValue("Car");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(1500);
            worksheet.Cells["B5"].PutValue(2500);

            // Создайте сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Добавьте поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Отобразить текущее значение ShowMemberPropertyTips
            Console.WriteLine("Current ShowMemberPropertyTips value: " + pivotTable.ShowMemberPropertyTips);

            // Изменить свойство ShowMemberPropertyTips
            pivotTable.ShowMemberPropertyTips = false;
            Console.WriteLine("ShowMemberPropertyTips set to: " + pivotTable.ShowMemberPropertyTips);

            // Вычислить данные и обновить сводную таблицу
            pivotTable.CalculateData();
            pivotTable.RefreshData();

            // Сохраните книгу
            workbook.Save("PivotTablePropertyShowMemberPropertyTipsDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


