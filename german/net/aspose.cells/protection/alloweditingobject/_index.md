---
title: "Protection.AllowEditingObject"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Schutz-Eigenschaft. Gibt an, ob der Benutzer Zeichenobjekte in einem geschützten Arbeitsblatt bearbeiten darf"
type: docs
url: /de/net/aspose.cells/protection/alloweditingobject/
---
## Protection.AllowEditingObject property

Stellt dar, ob der Benutzer Zeichenobjekte in einem geschützten Arbeitsblatt manipulieren darf.

```csharp
public bool AllowEditingObject { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowEditingObjectDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Schutzeinstellungen festlegen, wobei AllowEditingObject aktiviert ist
            Protection protection = worksheet.Protection;
            protection.AllowEditingObject = true;
            protection.AllowEditingContent = false; // Contrast with AllowEditingObject
            worksheet.Protect(ProtectionType.All);

            // Schutz-Flags prüfen
            Console.WriteLine("Protection Settings:");
            Console.WriteLine($"AllowEditingObject: {protection.AllowEditingObject}");
            Console.WriteLine($"AllowEditingContent: {protection.AllowEditingContent}");

            // Erstelle ein Textfeld (Objekt), um die Bearbeitung zu testen
            worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            
            // Speichere die Arbeitsmappe
            workbook.Save("ProtectionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


