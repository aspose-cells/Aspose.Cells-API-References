---
title: "PaginatedSaveOptions.IsFontSubstitutionCharGranularity"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PaginatedSaveOptions. Указывает, следует ли заменять шрифт символа только когда шрифт ячейки несовместим с ним"
type: docs
url: /ru/net/aspose.cells/paginatedsaveoptions/isfontsubstitutionchargranularity/
---
## PaginatedSaveOptions.IsFontSubstitutionCharGranularity property

Указывает, следует ли заменять шрифт символа только тогда, когда шрифт ячейки несовместим с ним.

```csharp
public bool IsFontSubstitutionCharGranularity { get; set; }
```

### Примечания

По умолчанию false. Сначала мы попробуем использовать шрифт по умолчанию из Workbook и PdfSaveOption/system для шрифта ячейки.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyIsFontSubstitutionCharGranularityDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue("Sample Text with Font Substitution");

            XpsSaveOptions saveOptions = new XpsSaveOptions
            {
                IsFontSubstitutionCharGranularity = true,
                DefaultFont = "Arial"
            };

            workbook.Save("FontSubstitutionDemo.xps", saveOptions);
        }
    }
}
```

### См. также

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


