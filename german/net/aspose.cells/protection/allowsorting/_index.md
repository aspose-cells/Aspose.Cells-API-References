---
title: "Protection.AllowSorting"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Schutz-Eigenschaft. Gibt an, ob die Sortieroption in einem geschützten Arbeitsblatt erlaubt ist"
type: docs
url: /de/net/aspose.cells/protection/allowsorting/
---
## Protection.AllowSorting property

Stellt dar, ob die Sortieroption in einem geschützten Arbeitsblatt erlaubt ist.

```csharp
public bool AllowSorting { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowSortingDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Arbeitsblattschutz aktivieren
            worksheet.Protect(ProtectionType.All);
            
            // Schutzeigenschaften festlegen, einschließlich AllowSorting
            Protection protection = worksheet.Protection;
            protection.AllowSorting = true;
            protection.AllowFiltering = true;
            protection.AllowEditingContent = false;

            // Schutzeinstellungen ausgeben
            Console.WriteLine("Protection Settings:");
            Console.WriteLine($"AllowSorting: {protection.AllowSorting}");
            Console.WriteLine($"AllowFiltering: {protection.AllowFiltering}");
            Console.WriteLine($"AllowEditingContent: {protection.AllowEditingContent}");

            // Sortierfähigkeit demonstrieren
            if (protection.AllowSorting)
            {
                Console.WriteLine("\nSorting is allowed on this protected worksheet");
            }
            else
            {
                Console.WriteLine("\nSorting is not allowed on this protected worksheet");
            }
        }
    }
}
```

### Siehe auch

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


