---
title: "PivotTable.EnableFieldDialog"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Указывает, доступен ли диалоговое окно полей PivotTable, когда пользователь дважды щёлкает поле PivotTable"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/enablefielddialog/
---
## PivotTable.EnableFieldDialog property

Указывает, доступно ли диалоговое окно поля сводной таблицы, когда пользователь дважды щёлкает поле сводной таблицы.

```csharp
public bool EnableFieldDialog { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyEnableFieldDialogDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            var cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // Создать сводную таблицу
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Продемонстрировать свойство EnableFieldDialog
            pivotTable.EnableFieldDialog = true;
            Console.WriteLine("EnableFieldDialog set to: " + pivotTable.EnableFieldDialog);

            // Измените свойство и проверьте
            pivotTable.EnableFieldDialog = false;
            Console.WriteLine("EnableFieldDialog changed to: " + pivotTable.EnableFieldDialog);

            // Сохраните книгу
            workbook.Save("PivotTable_EnableFieldDialog_Example.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


