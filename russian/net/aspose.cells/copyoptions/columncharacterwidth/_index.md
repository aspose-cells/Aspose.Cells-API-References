---
title: "CopyOptions.ColumnCharacterWidth"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CopyOptions. Указывает, копировать ли ширину столбца в единицах символов"
type: docs
url: /ru/net/aspose.cells/copyoptions/columncharacterwidth/
---
## CopyOptions.ColumnCharacterWidth property

Указывает, копировать ли ширину столбца в единицах символов.

```csharp
public bool ColumnCharacterWidth { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyColumnCharacterWidthDemo
    {
        public static void Run()
        {
            // Создайте исходную книгу с примерными данными
            Workbook srcWorkbook = new Workbook();
            Worksheet srcSheet = srcWorkbook.Worksheets[0];
            
            // Установите ширину столбца в символах для демонстрации
            srcSheet.Cells.SetColumnWidth(0, 20); // 20 characters wide
            
            // Добавьте некоторые образцы данных.
            srcSheet.Cells["A1"].PutValue("Sample Text");
            srcSheet.Cells["A2"].PutValue("Another Sample");
            
            // Создайте целевую книгу
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // Копировать с установленным ColumnCharacterWidth в true
            destSheet.Copy(srcSheet, new CopyOptions()
            {
                ColumnCharacterWidth = true
            });
            
            // Сохранить результат
            destWorkbook.Save("output_with_column_width.xlsx", SaveFormat.Xlsx);
            
            // Для сравнения скопируйте без ColumnCharacterWidth
            Workbook destWorkbook2 = new Workbook();
            Worksheet destSheet2 = destWorkbook2.Worksheets[0];
            
            destSheet2.Copy(srcSheet, new CopyOptions()
            {
                ColumnCharacterWidth = false
            });
            
            destWorkbook2.Save("output_without_column_width.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


