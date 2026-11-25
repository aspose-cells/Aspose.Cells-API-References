---
title: "Style.IsProtectionApplied"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Style. Indica se la formattazione di protezione deve essere applicata"
type: docs
url: /it/net/aspose.cells/style/isprotectionapplied/
---
## Style.IsProtectionApplied property

Indica se la formattazione di protezione deve essere applicata.

```csharp
public bool IsProtectionApplied { get; set; }
```

### Osservazioni

Solo per stile con nome.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsProtectionAppliedDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea un oggetto stile
            Style style = workbook.CreateStyle();
            
            // Imposta le proprietà di protezione
            style.IsLocked = true;
            style.IsFormulaHidden = true;
            style.IsProtectionApplied = true;
            
            // Applica lo stile a una cella
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            
            // Verifica le impostazioni di protezione
            Console.WriteLine("IsProtectionApplied: " + style.IsProtectionApplied);
            Console.WriteLine("IsLocked: " + style.IsLocked);
            Console.WriteLine("IsFormulaHidden: " + style.IsFormulaHidden);
            
            // Modifica le impostazioni di protezione
            style.IsProtectionApplied = false;
            Console.WriteLine("\nAfter changing IsProtectionApplied to false:");
            Console.WriteLine("IsProtectionApplied: " + style.IsProtectionApplied);
        }
    }
}
```

### Vedi anche

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


