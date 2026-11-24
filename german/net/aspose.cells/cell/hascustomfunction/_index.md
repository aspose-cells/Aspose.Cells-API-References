---
title: "Cell.HasCustomFunction"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Eigenschaft. Überprüft, ob in der Formel dieser Zelle eine benutzerdefinierte Funktion/unsupported function vorhanden ist."
type: docs
url: /de/net/aspose.cells/cell/hascustomfunction/
---
## Cell.HasCustomFunction property

Überprüft, ob es eine benutzerdefinierte Funktion (nicht unterstützte Funktion) in der Formel dieser Zelle gibt.

```csharp
public bool HasCustomFunction { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyHasCustomFunctionDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook wb = new Workbook();
            
            // Füge einen benutzerdefinierten Funktionsnamen hinzu
            NameCollection nc = wb.Worksheets.Names;
            nc[nc.Add("MyCustomFunc")].RefersTo = "=MYTESTFUNC()";
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Test mit integrierter Funktion
            Cell cell1 = cells[0, 0];
            cell1.Formula = "=SUM(A1:B1)";
            Console.WriteLine("HasCustomFunction (SUM): " + cell1.HasCustomFunction);
            
            // Test mit benutzerdefinierter Funktion
            Cell cell2 = cells[1, 0];
            cell2.Formula = "=MYTESTFUNC()";
            Console.WriteLine("HasCustomFunction (MYTESTFUNC): " + cell2.HasCustomFunction);
            
            // Test mit benanntem Bereich, der eine benutzerdefinierte Funktion enthält
            Cell cell3 = cells[2, 0];
            cell3.Formula = "=MyCustomFunc";
            Console.WriteLine("HasCustomFunction (Named Range): " + cell3.HasCustomFunction);
            
            // Test mit verschachtelter benutzerdefinierter Funktion
            Cell cell4 = cells[3, 0];
            cell4.Formula = "=SUM(MYTESTFUNC(), A1)";
            Console.WriteLine("HasCustomFunction (Nested): " + cell4.HasCustomFunction);
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


