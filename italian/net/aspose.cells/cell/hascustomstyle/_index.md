---
title: "Cell.HasCustomStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cell. Indica se questa cella ha impostazioni di stile personalizzate diverse da quelle predefinite ereditate dalla riga, colonna o cartella di lavoro corrispondente."
type: docs
url: /it/net/aspose.cells/cell/hascustomstyle/
---
## Cell.HasCustomStyle property

Indica se questa cella ha impostazioni di stile personalizzate (diverse da quelle predefinite ereditate dalla riga, colonna o cartella di lavoro corrispondente).

```csharp
public bool HasCustomStyle { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellPropertyHasCustomStyleDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e accedi al primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Check HasCustomStyle");

            // Visualizza il valore iniziale di HasCustomState (eredita lo stile predefinito)
            Console.WriteLine("Initial HasCustomStyle: " + cell.HasCustomStyle);

            // Crea uno stile personalizzato e applicalo alla cella
            Style customStyle = workbook.CreateStyle();
            customStyle.Font.IsBold = true;
            cell.SetStyle(customStyle);

            // Verifica che HasCustomStyle sia true dopo la modifica dello stile
            Console.WriteLine("After applying custom style - HasCustomStyle: " + cell.HasCustomStyle);

            // Salva la cartella di lavoro con lo stile personalizzato applicato
            workbook.Save("CellCustomStyleDemo.xlsx");

            // Reimposta lo stile della cella allo stile predefinito della cartella di lavoro
            Style defaultStyle = workbook.DefaultStyle;
            cell.SetStyle(defaultStyle);

            // Verifica che HasCustomStyle sia false dopo il ripristino al valore predefinito
            Console.WriteLine("After resetting to default style - HasCustomStyle: " + cell.HasCustomStyle);
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


