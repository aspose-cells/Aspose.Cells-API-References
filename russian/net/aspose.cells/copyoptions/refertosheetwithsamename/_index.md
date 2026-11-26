---
title: "CopyOptions.ReferToSheetWithSameName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CopyOptions. В MS Excel при копировании формул, которые ссылаются на другие листы, при копировании листа в другой лист скопированные формулы должны ссылаться на исходную книгу. Однако в некоторых ситуациях пользователю может потребоваться, чтобы скопированные формулы ссылались на листы с тем же именем в той же книге, например когда эти листы уже были скопированы до этой операции копирования; тогда это свойство должно быть установлено в true."
type: docs
url: /ru/net/aspose.cells/copyoptions/refertosheetwithsamename/
---
## CopyOptions.ReferToSheetWithSameName property

В MS Excel при копировании формул, которые ссылаются на другие листы, при копировании листа в другой, скопированные формулы должны ссылаться на исходную книгу. Однако в некоторых ситуациях пользователю может потребоваться, чтобы скопированные формулы ссылались на листы с тем же именем в той же книге, например когда эти листы уже были скопированы до этой операции копирования; в этом случае свойство следует оставить истинным.

```csharp
public bool ReferToSheetWithSameName { get; set; }
```

### Примечания

Значение по умолчанию — true.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyReferToSheetWithSameNameDemo
    {
        public static void Run()
        {
            // Создайте шаблон книги с образцовыми данными
            Workbook templateWorkbook = new Workbook();
            Worksheet templateSheet1 = templateWorkbook.Worksheets[0];
            templateSheet1.Name = "Data";
            templateSheet1.Cells["A1"].PutValue("Value");
            templateSheet1.Cells["A2"].PutValue(10);
            templateSheet1.Cells["A3"].PutValue(20);
            
            Worksheet templateSheet2 = templateWorkbook.Worksheets.Add("Summary");
            templateSheet2.Cells["B2"].Formula = "=SUM(Data!A2:A3)";

            // Создайте результирующую книгу
            Workbook outputWorkbook = new Workbook();
            outputWorkbook.Worksheets.Clear();

            // Скопируйте листы с включённым параметром ReferToSheetWithSameName
            foreach (Worksheet sheet in templateWorkbook.Worksheets)
            {
                outputWorkbook.Worksheets.Add(sheet.Name);
                CopyOptions options = new CopyOptions();
                options.ReferToSheetWithSameName = true;
                outputWorkbook.Worksheets[sheet.Name].Copy(sheet, options);
            }

            // Проверьте, что формула ссылается на правильный лист
            Console.WriteLine("Formula in output workbook: " + 
                outputWorkbook.Worksheets["Summary"].Cells["B2"].Formula);
        }
    }
}
```

### См. также

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


