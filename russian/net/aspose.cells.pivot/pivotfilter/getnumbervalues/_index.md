---
title: "PivotFilter.GetNumberValues"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotFilter. Получает значения числового фильтра"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfilter/getnumbervalues/
---
## PivotFilter.GetNumberValues method

Получает значения числового фильтра.

```csharp
public double[] GetNumberValues()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterMethodGetNumberValuesDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            sheet.Cells["A1"].Value = "Fruit";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["A3"].Value = "Orange";
            sheet.Cells["A4"].Value = "Banana";
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["B2"].Value = 5;
            sheet.Cells["B3"].Value = 3;
            sheet.Cells["B4"].Value = 2;

            // Создать сводную таблицу
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Применить фильтр значений
            pivotTable.RowFields[0].FilterByValue(0, PivotFilterType.ValueLessThan, 4, 0);
            
            // Получить и отобразить значения фильтра
            PivotFilter filter = pivotTable.RowFields[0].GetFilters()[0];
            double[] numberValues = filter.GetNumberValues();
            
            Console.WriteLine("Filter Type: " + filter.FilterType);
            Console.WriteLine("Number Values: " + string.Join(", ", numberValues));
        }
    }
}
```

### См. также

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


