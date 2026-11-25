---
title: "Cell.HasCustomFunction"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cell. Verifica se esiste una funzione personalizzata non supportata nella formula di questa cella."
type: docs
url: /it/net/aspose.cells/cell/hascustomfunction/
---
## Cell.HasCustomFunction property

Verifica se nella formula di questa cella è presente una funzione personalizzata (funzione non supportata).

```csharp
public bool HasCustomFunction { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyHasCustomFunctionDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook wb = new Workbook();
            
            // Aggiungi un nome di funzione personalizzata
            NameCollection nc = wb.Worksheets.Names;
            nc[nc.Add("MyCustomFunc")].RefersTo = "=MYTESTFUNC()";
            
            // Accedi al primo foglio di lavoro
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Test con funzione integrata
            Cell cell1 = cells[0, 0];
            cell1.Formula = "=SUM(A1:B1)";
            Console.WriteLine("HasCustomFunction (SUM): " + cell1.HasCustomFunction);
            
            // Test con funzione personalizzata
            Cell cell2 = cells[1, 0];
            cell2.Formula = "=MYTESTFUNC()";
            Console.WriteLine("HasCustomFunction (MYTESTFUNC): " + cell2.HasCustomFunction);
            
            // Test con intervallo denominato contenente funzione personalizzata
            Cell cell3 = cells[2, 0];
            cell3.Formula = "=MyCustomFunc";
            Console.WriteLine("HasCustomFunction (Named Range): " + cell3.HasCustomFunction);
            
            // Test con funzione personalizzata annidata
            Cell cell4 = cells[3, 0];
            cell4.Formula = "=SUM(MYTESTFUNC(), A1)";
            Console.WriteLine("HasCustomFunction (Nested): " + cell4.HasCustomFunction);
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


