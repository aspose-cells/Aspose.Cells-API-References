---
title: "Style.IsBorderApplied"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Style. Indica se la formattazione del bordo deve essere applicata"
type: docs
url: /it/net/aspose.cells/style/isborderapplied/
---
## Style.IsBorderApplied property

Indica se la formattazione del bordo deve essere applicata.

```csharp
public bool IsBorderApplied { get; set; }
```

### Osservazioni

Solo per stile con nome.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsBorderAppliedDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea uno stile personalizzato
            Style style = workbook.CreateStyle();
            
            // Applica le impostazioni del bordo allo stile
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Black;
            
            // Verifica se il bordo è applicato
            Console.WriteLine("IsBorderApplied before setting: " + style.IsBorderApplied);
            
            // Imposta esplicitamente IsBorderApplied su true
            style.IsBorderApplied = true;
            
            // Applica lo stile a una cella
            worksheet.Cells["A1"].SetStyle(style);
            
            // Verifica l'applicazione del bordo
            Console.WriteLine("IsBorderApplied after setting: " + style.IsBorderApplied);
            
            // Salva la cartella di lavoro
            workbook.Save("IsBorderAppliedDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


