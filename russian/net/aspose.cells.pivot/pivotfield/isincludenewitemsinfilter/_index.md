---
title: "PivotField.IsIncludeNewItemsInFilter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotField. Указывает, следует ли включать новые элементы в поле при ручной фильтрации. Значение по умолчанию — false"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/isincludenewitemsinfilter/
---
## PivotField.IsIncludeNewItemsInFilter property

Указывает, следует ли включать новые элементы в поле при ручной фильтрации. Значение по умолчанию — false.

```csharp
public bool IsIncludeNewItemsInFilter { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsIncludeNewItemsInFilterDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 150;

            // Создать сводную таблицу
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Добавить поле строки
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Добавить поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Получите поле сводной таблицы и установите IsIncludeNewItemsInFilter
            PivotField field = pivotTable.RowFields[0];
            field.IsIncludeNewItemsInFilter = true;
            
            // Вывести значение свойства
            Console.WriteLine("IsIncludeNewItemsInFilter: " + field.IsIncludeNewItemsInFilter);
            
            // Сохраните книгу
            workbook.Save("PivotFieldPropertyIsIncludeNewItemsInFilterDemo_out.xlsx");
        }
    }
}
```

### См. также

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


