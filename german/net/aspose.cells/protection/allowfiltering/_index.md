---
title: "Protection.AllowFiltering"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Protection-Eigenschaft. Gibt an, ob der Benutzer die Verwendung eines AutoFilters, der vor dem Schutz des Blatts erstellt wurde, nutzen darf."
type: docs
url: /de/net/aspose.cells/protection/allowfiltering/
---
## Protection.AllowFiltering property

Stellt dar, ob der Benutzer einen AutoFilter, der vor dem Schutz des Blatts erstellt wurde, verwenden darf.

```csharp
public bool AllowFiltering { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowFilteringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Arbeitsblattschutz aktivieren
            worksheet.Protect(ProtectionType.All);
            
            // Setzen Sie AllowFiltering auf true
            worksheet.Protection.AllowFiltering = true;
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
            
            // Überprüfen Sie, ob die Eigenschaft korrekt gespeichert wurde
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("AllowFiltering: " + 
                loadedWorkbook.Worksheets[0].Protection.AllowFiltering);
        }
    }
}
```

### Siehe auch

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


