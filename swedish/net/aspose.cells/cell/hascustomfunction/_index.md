---
title: "Cell.HasCustomFunction"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-egenskap. Kontrollerar om det finns en anpassad funktion eller en funktion som inte stöds i den här cellens formel"
type: docs
url: /sv/net/aspose.cells/cell/hascustomfunction/
---
## Cell.HasCustomFunction property

Kontrollerar om det finns en anpassad funktion (ej stödd funktion) i cellens formel.

```csharp
public bool HasCustomFunction { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyHasCustomFunctionDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook wb = new Workbook();
            
            // Lägg till ett anpassat funktionsnamn
            NameCollection nc = wb.Worksheets.Names;
            nc[nc.Add("MyCustomFunc")].RefersTo = "=MYTESTFUNC()";
            
            // Kom åt första arbetsbladet
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Testa med inbyggd funktion
            Cell cell1 = cells[0, 0];
            cell1.Formula = "=SUM(A1:B1)";
            Console.WriteLine("HasCustomFunction (SUM): " + cell1.HasCustomFunction);
            
            // Testa med anpassad funktion
            Cell cell2 = cells[1, 0];
            cell2.Formula = "=MYTESTFUNC()";
            Console.WriteLine("HasCustomFunction (MYTESTFUNC): " + cell2.HasCustomFunction);
            
            // Testa med namngivet område som innehåller en anpassad funktion
            Cell cell3 = cells[2, 0];
            cell3.Formula = "=MyCustomFunc";
            Console.WriteLine("HasCustomFunction (Named Range): " + cell3.HasCustomFunction);
            
            // Testa med nästlad anpassad funktion
            Cell cell4 = cells[3, 0];
            cell4.Formula = "=SUM(MYTESTFUNC(), A1)";
            Console.WriteLine("HasCustomFunction (Nested): " + cell4.HasCustomFunction);
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


