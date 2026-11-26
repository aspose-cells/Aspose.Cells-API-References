---
title: "CopyOptions.CopyNames"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CopyOptions. Указывает, копировать ли имена"
type: docs
url: /ru/net/aspose.cells/copyoptions/copynames/
---
## CopyOptions.CopyNames property

Указывает, копировать ли имена.

```csharp
public bool CopyNames { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyCopyNamesDemo
    {
        public static void Run()
        {
            // Создайте исходную книгу с именованными диапазонами
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            
            // Создайте именованный диапазон в исходной книге
            sourceSheet.Cells["A1"].PutValue("Test Value");
            int index = sourceWorkbook.Worksheets.Names.Add("SourceName");
            sourceWorkbook.Worksheets.Names[index].RefersTo = "=Sheet1!$A$1";

            // Создайте целевую книгу
            Workbook destWorkbook = new Workbook();
            
            // Копировать лист с CopyNames=true
            destWorkbook.Worksheets[0].Copy(sourceSheet, new CopyOptions { CopyNames = true });

            // Проверьте, что именованный диапазон был скопирован
            Name copiedName = destWorkbook.Worksheets.Names["SourceName"];
            if (copiedName != null)
            {
                Console.WriteLine("Named range copied successfully: " + copiedName.RefersTo);
            }
            else
            {
                Console.WriteLine("Named range was not copied");
            }
        }
    }
}
```

### См. также

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


