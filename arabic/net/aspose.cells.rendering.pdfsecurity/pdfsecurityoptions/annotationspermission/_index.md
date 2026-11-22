---
title: "PdfSecurityOptions.AnnotationsPermission"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PdfSecurityOptions. تشير إلى ما إذا كان يُسمح بإضافة أو تعديل تعليقات النص وتعبئة حقول النماذج التفاعلية"
type: docs
url: /ar/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/annotationspermission/
---
## PdfSecurityOptions.AnnotationsPermission property

يُشير إلى ما إذا كان يُسمح بإضافة أو تعديل التعليقات النصية، وملء حقول النماذج التفاعلية.

```csharp
public bool AnnotationsPermission { get; set; }
```

### ملاحظات

إذا كان [`ModifyDocumentPermission`](../modifydocumentpermission/) مُحددًا أيضًا، يتم إنشاء أو تعديل حقول النماذج التفاعلية (بما في ذلك حقول التوقيع).

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyAnnotationsPermissionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Test PDF with Annotations Permission";

            PdfSaveOptions saveOptions = new PdfSaveOptions();
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();

            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            securityOptions.AnnotationsPermission = true;

            saveOptions.SecurityOptions = securityOptions;
            workbook.Save("AnnotationsPermissionDemo.pdf", saveOptions);

            Console.WriteLine("PDF created with annotations permission enabled.");
        }
    }
}
```

### انظر أيضًا

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


