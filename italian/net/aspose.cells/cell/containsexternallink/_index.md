---
title: "Cell.ContainsExternalLink"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cell. Indica se questa cella contiene un link esterno. Si applica solo quando la cella è una cella di formula."
type: docs
url: /it/net/aspose.cells/cell/containsexternallink/
---
## Cell.ContainsExternalLink property

Indica se questa cella contiene un collegamento esterno. Si applica solo quando la cella è una cella di formula.

```csharp
public bool ContainsExternalLink { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyContainsExternalLinkDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio e un link esterno
            sheet.Cells["A1"].PutValue("External Link:");
            sheet.Cells["B1"].Formula = "=HYPERLINK(\"https://www.aspose.com\", \"Aspose\")";
            
            // Verifica se le celle contengono link esterni
            Console.WriteLine("A1 ContainsExternalLink: " + sheet.Cells["A1"].ContainsExternalLink);
            Console.WriteLine("B1 ContainsExternalLink: " + sheet.Cells["B1"].ContainsExternalLink);
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


