---
title: "PivotTable.IsExcel2003Compatible"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Указывает, совместима ли PivotTable с Excel2003 при обновлении PivotTable; если true, строка должна быть длиной не более 255 символов, поэтому если строка длиннее 255 символов, она будет усечена. Если false, на строку не будет наложено вышеуказанное ограничение. Значение по умолчанию — true."
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/isexcel2003compatible/
---
## PivotTable.IsExcel2003Compatible property

Указывает, совместима ли сводная таблица с Excel2003 при её обновлении; если true, строка должна быть длиной не более 255 символов, иначе будет усечена. Если false, ограничение не применяется. Значение по умолчанию — true.

```csharp
public bool IsExcel2003Compatible { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyIsExcel2003CompatibleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook wb = new Workbook();
            
            // Добавьте лист и заполните его образцовыми данными
            Worksheet dataSheet = wb.Worksheets[0];
            dataSheet.Name = "Data";
            dataSheet.Cells["A1"].Value = "Product";
            dataSheet.Cells["B1"].Value = "Description";
            dataSheet.Cells["C1"].Value = "Status";
            dataSheet.Cells["D1"].Value = "Date";
            
            // Добавить строки примерных данных
            dataSheet.Cells["A2"].Value = "Product1";
            dataSheet.Cells["B2"].Value = "Short description";
            dataSheet.Cells["C2"].Value = "Active";
            dataSheet.Cells["D2"].Value = DateTime.Now;
            
            dataSheet.Cells["A3"].Value = "Product2";
            dataSheet.Cells["B3"].Value = "Very long description that exceeds Excel 2003 limits when used in pivot tables";
            dataSheet.Cells["C3"].Value = "Inactive";
            dataSheet.Cells["D3"].Value = DateTime.Now.AddDays(-1);

            // Добавить сводную таблицу
            Worksheet pivotSheet = wb.Worksheets.Add("PivotTable");
            int pivotIndex = pivotSheet.PivotTables.Add("PivotTable", "A1:D3", "A4", false);
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            
            // Настроить поля сводной таблицы
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Description
            
            // Установить режим совместимости
            pivotTable.IsExcel2003Compatible = false; // Allow longer text in pivot tables
            
            // Обновить и вычислить данные
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Сохраните книгу
            wb.Save("PivotTableExcel2003CompatibilityDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


