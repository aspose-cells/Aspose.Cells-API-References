---
title: "Protection.AllowEditingContent"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Protection-Eigenschaft. Gibt an, ob der Benutzer Inhalte gesperrter Zellen in einem geschützten Arbeitsblatt bearbeiten darf."
type: docs
url: /de/net/aspose.cells/protection/alloweditingcontent/
---
## Protection.AllowEditingContent property

Stellt dar, ob der Benutzer den Inhalt gesperrter Zellen in einem geschützten Arbeitsblatt bearbeiten darf.

```csharp
public bool AllowEditingContent { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowEditingContentDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Schütze das Arbeitsblatt mit einem Passwort
            worksheet.Protect(ProtectionType.All, "password", null);
            
            // Überprüfen und Anzeigen der AllowEditingContent-Eigenschaft
            Console.WriteLine("AllowEditingContent before setting: " + worksheet.Protection.AllowEditingContent);
            
            // Ändern der AllowEditingContent-Eigenschaft
            worksheet.Protection.AllowEditingContent = true;
            
            // Überprüfen und Anzeigen der aktualisierten Eigenschaft
            Console.WriteLine("AllowEditingContent after setting: " + worksheet.Protection.AllowEditingContent);
            
            // Speichere die Arbeitsmappe
            workbook.Save("ProtectionPropertyAllowEditingContentDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


