---
title: "PdfSecurityOptions.UserPassword"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PdfSecurityOptions-Eigenschaft. Gibt das Benutzerpasswort zurück oder legt es fest, das zum Öffnen des verschlüsselten PDF-Dokuments erforderlich ist."
type: docs
url: /de/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/userpassword/
---
## PdfSecurityOptions.UserPassword property

Liest oder legt das Benutzerkennwort fest, das zum Öffnen des verschlüsselten PDF-Dokuments erforderlich ist.

```csharp
public string UserPassword { get; set; }
```

### Hinweise

Das Besitzerpasswort oder das Benutzerpasswort wird zum Öffnen eines verschlüsselten PDF-Dokuments für die Anzeige benötigt.

Das Benutzerpasswort kann null oder ein leerer String sein; in diesem Fall wird beim Öffnen des PDF-Dokuments kein Passwort vom Benutzer verlangt.

Das Öffnen des Dokuments mit dem korrekten Besitzerpasswort ermöglicht vollen Zugriff auf das Dokument.

Das Öffnen des Dokuments mit dem korrekten Benutzerpasswort (oder das Öffnen eines Dokuments ohne Benutzerpasswort) gewährt eingeschränkten Zugriff gemäß den angegebenen Berechtigungen.

### Beispiele

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

### Siehe auch

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


