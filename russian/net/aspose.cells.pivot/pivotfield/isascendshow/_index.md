---
title: "PivotField.IsAscendShow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotField. Указывает, отображается ли указанное поле PivotTable автоматически в порядке возрастания"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/isascendshow/
---
## PivotField.IsAscendShow property

Указывает, отображается ли указанное поле сводной таблицы автоматически в порядке возрастания.

```csharp
[Obsolete("Use  PivotField.Top10AutoShowSettings.IsTop property or PivotField.Top10AutoShow() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsAscendShow { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство PivotField.Top10AutoShowSettings.IsTop или метод PivotField.Top10AutoShow(). Этот метод будет удалён через 12 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsAscendShowDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 150;

            // Добавьте сводную таблицу
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Добавить поле строки
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            PivotField rowField = pivotTable.RowFields[0];
            
            // Установить свойство IsAscendShow
            rowField.IsAscendShow = true;
            Console.WriteLine("IsAscendShow (Row Field): " + rowField.IsAscendShow);
            
            // Добавить поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pivotTable.DataFields[0];
            
            // Установить свойство IsAscendShow
            dataField.IsAscendShow = false;
            Console.WriteLine("IsAscendShow (Data Field): " + dataField.IsAscendShow);
            
            // Обновить сводную таблицу
            pivotTable.RefreshData();
            pivotTable.CalculateData();
        }
    }
}
```

### См. также

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


