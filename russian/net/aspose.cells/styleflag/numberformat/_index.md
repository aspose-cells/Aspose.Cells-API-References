---
title: "StyleFlag.NumberFormat"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство StyleFlag. Будет применена настройка числового формата"
type: docs
url: /ru/net/aspose.cells/styleflag/numberformat/
---
## StyleFlag.NumberFormat property

Настройка числового формата будет применена.

```csharp
public bool NumberFormat { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyNumberFormatDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Установить значение ячейки
            sheet.Cells[0, 0].Value = 1234.56;
            
            // Создать стиль пользовательского числового формата
            Style style = workbook.CreateStyle();
            style.Custom = "_-€ #,##0.00;[Red]_-€ -#,##0.00";
            
            // Применить только числовой формат с помощью StyleFlag
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.NumberFormat = true;
            
            // Применить стиль к диапазону ячеек (полностью указать тип Range)
            Aspose.Cells.Range range = sheet.Cells.CreateRange(0, 0, 1, 1);
            range.ApplyStyle(style, styleFlag);
            
            // Сохранить и проверить
            workbook.Save("output_number_format.ods");
            
            // Перезагрузить для проверки
            Workbook verifyWorkbook = new Workbook("output_number_format.ods");
            Worksheet verifySheet = verifyWorkbook.Worksheets[0];
            Console.WriteLine("Applied Number Format: " + verifySheet.Cells["A1"].GetStyle().Custom);
        }
    }
}
```

### См. также

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


