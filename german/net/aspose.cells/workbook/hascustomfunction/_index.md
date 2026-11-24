---
title: "Workbook.HasCustomFunction"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Eigenschaft. Erkennt, ob in diesem Arbeitsbuch eine benutzerdefinierte Funktion verwendet wird, z. B. in Zellformeln oder definierten Namen"
type: docs
url: /de/net/aspose.cells/workbook/hascustomfunction/
---
## Workbook.HasCustomFunction property

Ermittelt, ob in dieser Arbeitsmappe benutzerdefinierte Funktionen verwendet werden, z. B. in Zellformeln oder definierten Namen...

```csharp
public bool HasCustomFunction { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyHasCustomFunctionDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook wb = new Workbook();
            
            // Eine Standardformel zu einem Namen hinzufügen
            NameCollection names = wb.Worksheets.Names;
            int index = names.Add("StandardName");
            names[index].RefersTo = "=SUM(Sheet1!$A$1:$A$2)";
            Console.WriteLine($"Workbook has custom function (should be false): {wb.HasCustomFunction}");

            // Eine benutzerdefinierte Funktion zu einem Namen hinzufügen
            index = names.Add("CustomName");
            names[index].RefersTo = "=MYFUNC()";
            Console.WriteLine($"Workbook has custom function (should be true): {wb.HasCustomFunction}");

            // Test mit Zellformeln
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Standardfunktion in Zelle
            cells["A1"].Formula = "=SUM(B1:B2)";
            Console.WriteLine($"Cell has custom function (should be false): {cells["A1"].HasCustomFunction}");

            // Benutzerdefinierte Funktion in Zelle
            cells["A2"].Formula = "=MYFUNC(B1)";
            Console.WriteLine($"Cell has custom function (should be true): {cells["A2"].HasCustomFunction}");

            // Verweis auf Namen mit benutzerdefinierter Funktion
            cells["A3"].Formula = "=CustomName";
            Console.WriteLine($"Cell has custom function (should be true): {cells["A3"].HasCustomFunction}");

            // Kombinierte benutzerdefinierte Funktionen
            cells["A4"].Formula = "=MYFUNC(CustomName)";
            Console.WriteLine($"Cell has custom function (should be true): {cells["A4"].HasCustomFunction}");
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


