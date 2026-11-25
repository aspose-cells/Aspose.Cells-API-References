---
title: "Style.IsFontApplied"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Style. Indica se la formattazione del carattere deve essere applicata"
type: docs
url: /it/net/aspose.cells/style/isfontapplied/
---
## Style.IsFontApplied property

Indica se la formattazione del carattere deve essere applicata.

```csharp
public bool IsFontApplied { get; set; }
```

### Osservazioni

Solo per stile con nome.

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyIsFontAppliedDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi a una cella dal foglio di lavoro
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");
            
            // Ottieni lo stile della cella
            Style style = cell.GetStyle();
            
            // Applica le impostazioni del carattere
            style.Font.Name = "Times New Roman";
            style.Font.Size = 14;
            style.Font.Color = Color.Blue;
            
            // Abilita l'applicazione del carattere
            style.IsFontApplied = true;
            
            // Imposta lo stile modificato nuovamente nella cella
            cell.SetStyle(style);
            
            // Salva la cartella di lavoro
            workbook.Save("FontAppliedDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


