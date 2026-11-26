---
title: "PdfSecurityOptions.AssembleDocumentPermission"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PdfSecurityOptions. Указывает, разрешено ли собирать документ, вставлять, вращать или удалять страницы и создавать закладки или миниатюры, даже если ModifyDocumentPermission отключено."
type: docs
url: /ru/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/assembledocumentpermission/
---
## PdfSecurityOptions.AssembleDocumentPermission property

Указывает, разрешено ли собирать документ (вставлять, вращать или удалять страницы и создавать закладки или миниатюры), даже если [`ModifyDocumentPermission`](../modifydocumentpermission/) отключено.

```csharp
public bool AssembleDocumentPermission { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyAssembleDocumentPermissionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Test PDF Security";

            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();

            pdfSecurityOptions.OwnerPassword = "owner123";
            pdfSecurityOptions.UserPassword = "user123";
            pdfSecurityOptions.AssembleDocumentPermission = false;
            pdfSecurityOptions.PrintPermission = true;

            pdfSaveOptions.SecurityOptions = pdfSecurityOptions;
            workbook.Save("secured_document.pdf", pdfSaveOptions);

            Console.WriteLine("PDF created with assemble document permission disabled.");
        }
    }
}
```

### См. также

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


