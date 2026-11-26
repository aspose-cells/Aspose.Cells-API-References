---
title: "Worksheet.Workbook"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Получает объект книги, содержащий этот лист"
type: docs
url: /ru/net/aspose.cells/worksheet/workbook/
---
## Worksheet.Workbook property

Получает объект книги, содержащий этот лист.

```csharp
public Workbook Workbook { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyWorkbookDemo
    {
        public static void Run()
        {
            // Создайте исходную книгу и получите лист
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            
            // Добавьте примерные данные в исходный лист
            sourceSheet.Cells["A1"].PutValue("Sample Data");
            sourceSheet.Cells["A2"].PutValue(100);
            sourceSheet.Cells["A3"].PutValue(200);
            
            // Создайте целевую книгу
            Workbook destWorkbook = new Workbook();
            
            // Скопируйте тему из исходной книги, используя свойство Worksheet.Workbook
            destWorkbook.CopyTheme(sourceSheet.Workbook);
            
            // Получите доступ к целевому листу и скопируйте данные
            Worksheet destSheet = destWorkbook.Worksheets[0];
            Aspose.Cells.Range sourceRange = sourceSheet.Cells.CreateRange("A1:A3");
            Aspose.Cells.Range destRange = destSheet.Cells.CreateRange("A1:A3");
            
            // Скопируйте данные с форматированием
            destRange.Copy(sourceRange);
            
            // Сохранить целевую книгу
            destWorkbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [Workbook](../../workbook/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


