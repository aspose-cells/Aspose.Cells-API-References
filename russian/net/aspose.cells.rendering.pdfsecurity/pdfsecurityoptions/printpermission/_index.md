---
title: "PdfSecurityOptions.PrintPermission"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PdfSecurityOptions. Указывает, разрешено ли печатать документ"
type: docs
url: /ru/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/printpermission/
---
## PdfSecurityOptions.PrintPermission property

Указывает, разрешено ли печатать документ.

```csharp
public bool PrintPermission { get; set; }
```

### Примечания

Возможно, не наивысшего качества, в зависимости от того, установлен ли также [`FullQualityPrintPermission`](../fullqualityprintpermission/).

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyPrintPermissionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Test Print Permission";

            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();

            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            securityOptions.PrintPermission = true;

            pdfSaveOptions.SecurityOptions = securityOptions;
            workbook.Save("PrintPermissionDemo.pdf", pdfSaveOptions);

            Console.WriteLine("PDF created with print permission enabled.");
        }
    }
}
```

### См. также

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


