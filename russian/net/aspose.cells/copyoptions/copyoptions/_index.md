---
title: "CopyOptions.CopyOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор CopyOptions. Конструктор CopyOptions"
type: docs
url: /ru/net/aspose.cells/copyoptions/copyoptions/
---
## CopyOptions constructor

Конструктор CopyOptions.

```csharp
public CopyOptions()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте лист и получите первый лист
            Worksheet sourceSheet = workbook.Worksheets[0];
            Worksheet destSheet = workbook.Worksheets[workbook.Worksheets.Add()];
            
            // Добавьте примерные данные в исходный лист
            sourceSheet.Cells["A1"].PutValue("Source Data");
            sourceSheet.Cells["A2"].PutValue(100);
            sourceSheet.Cells["A3"].PutValue(200);
            sourceSheet.Cells["A4"].PutValue(300);
            
            // Создайте CopyOptions, используя конструктор
            CopyOptions options = new CopyOptions();
            options.ReferToDestinationSheet = true;
            
            // Скопировать строки с параметрами
            destSheet.Cells.CopyRows(sourceSheet.Cells, 0, 0, sourceSheet.Cells.MaxDisplayRange.RowCount, options);
            
            // Сохраните книгу
            workbook.Save("CopyOptionsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


