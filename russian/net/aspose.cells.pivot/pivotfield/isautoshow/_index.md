---
title: "PivotField.IsAutoShow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotField. Указывает, отображается ли указанное поле PivotTable автоматически"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/isautoshow/
---
## PivotField.IsAutoShow property

Указывает, отображается ли указанное поле PivotTable автоматически.

```csharp
[Obsolete("Use  PivotField.Top10AutoShowSettings.IsAutoShow property  or PivotField.Top10AutoShow() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsAutoShow { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство PivotField.Top10AutoShowSettings.IsAutoShow или метод PivotField.Top10AutoShow(). Этот метод будет удалён через 12 месяцев, начиная с сентября 2026 года. Компания Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsAutoShowDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["A4"].Value = "Orange";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // Добавьте сводную таблицу
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Добавить поле строки
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Добавьте поле данных и настройте IsAutoShow
            int dataFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pivotTable.DataFields[dataFieldIndex];
            
            // Включите AutoShow и настройте параметры
            dataField.IsAutoShow = true;
            dataField.AutoShowCount = 2;
            dataField.AutoShowField = 0; // Index of the field to auto show
            dataField.IsAscendShow = true;
            
            // Вычислить данные
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Выведите значение свойства IsAutoShow
            Console.WriteLine("IsAutoShow property value: " + dataField.IsAutoShow);
            
            // Сохраните книгу
            workbook.Save("PivotFieldPropertyIsAutoShowDemo_out.xlsx");
        }
    }
}
```

### См. также

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


