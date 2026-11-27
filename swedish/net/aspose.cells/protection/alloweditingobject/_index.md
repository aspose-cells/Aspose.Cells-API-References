---
title: "Protection.AllowEditingObject"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Protection egenskap. Anger om användaren får manipulera ritobjekt på ett skyddat kalkylblad"
type: docs
url: /sv/net/aspose.cells/protection/alloweditingobject/
---
## Protection.AllowEditingObject property

Representerar om användaren får manipulera ritobjekt på ett skyddat kalkylblad.

```csharp
public bool AllowEditingObject { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowEditingObjectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ställ in skyddsinställningar med AllowEditingObject aktiverat
            Protection protection = worksheet.Protection;
            protection.AllowEditingObject = true;
            protection.AllowEditingContent = false; // Contrast with AllowEditingObject
            worksheet.Protect(ProtectionType.All);

            // Kontrollera skyddsflaggor
            Console.WriteLine("Protection Settings:");
            Console.WriteLine($"AllowEditingObject: {protection.AllowEditingObject}");
            Console.WriteLine($"AllowEditingContent: {protection.AllowEditingContent}");

            // Skapa en textruta (objekt) för att testa redigering
            worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            
            // Spara arbetsboken
            workbook.Save("ProtectionDemo.xlsx");
        }
    }
}
```

### Se även

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


