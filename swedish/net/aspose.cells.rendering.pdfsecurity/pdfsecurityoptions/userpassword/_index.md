---
title: "PdfSecurityOptions.UserPassword"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PdfSecurityOptions-egenskap. Hämtar eller anger användarlösenordet som krävs för att öppna det krypterade PDF-dokumentet"
type: docs
url: /sv/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/userpassword/
---
## PdfSecurityOptions.UserPassword property

Hämtar eller anger användarlösenordet som krävs för att öppna det krypterade PDF-dokumentet.

```csharp
public string UserPassword { get; set; }
```

### Anmärkningar

Ägarlösenordet eller användarlösenordet kommer att krävas för att öppna ett krypterat PDF-dokument för visning.

Användarlösenordet kan vara null eller en tom sträng; i så fall krävs inget lösenord från användaren när PDF-dokumentet öppnas.

Att öppna dokumentet med rätt ägarlösenord ger full åtkomst till dokumentet.

Att öppna dokumentet med rätt användarlösenord (eller öppna ett dokument som inte har något användarlösenord) ger begränsad åtkomst enligt de angivna behörigheterna.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyUserPasswordDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Protected PDF with User Password";

            PdfSaveOptions saveOptions = new PdfSaveOptions();
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();
            
            securityOptions.UserPassword = "user123";
            securityOptions.OwnerPassword = "owner456";
            securityOptions.PrintPermission = true;
            
            saveOptions.SecurityOptions = securityOptions;
            workbook.Save("ProtectedWithUserPassword.pdf", saveOptions);
            
            Console.WriteLine("PDF created with user password protection.");
        }
    }
}
```

### Se även

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


