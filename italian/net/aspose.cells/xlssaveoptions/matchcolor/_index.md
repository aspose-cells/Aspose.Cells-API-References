---
title: "XlsSaveOptions.MatchColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà XlsSaveOptions. Indica se abbinare il colore del carattere poiché nella tavolozza standard ci sono 56 colori"
type: docs
url: /it/net/aspose.cells/xlssaveoptions/matchcolor/
---
## XlsSaveOptions.MatchColor property

Indica se abbinare il colore del carattere poiché ci sono 56 colori nella tavolozza standard.

```csharp
public bool MatchColor { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class XlsSaveOptionsPropertyMatchColorDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro e accedi al primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi alla cella B2 e imposta del testo con un colore del carattere specifico
            Cell cellB2 = worksheet.Cells["B2"];
            cellB2.PutValue("Sample Text");
            
            // Imposta il colore del carattere su blu
            Style style = cellB2.GetStyle();
            style.Font.Color = Color.Blue;
            cellB2.SetStyle(style);

            // Crea le opzioni di salvataggio con MatchColor impostato su true
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            saveOptions.MatchColor = true;

            // Salva la cartella di lavoro con le opzioni
            workbook.Save("output.xls", saveOptions);

            // Ricarica il file salvato per verificare che il colore sia stato preservato
            Workbook savedWorkbook = new Workbook("output.xls");
            Cell savedCellB2 = savedWorkbook.Worksheets[0].Cells["B2"];
            
            // Verifica che il colore del carattere sia ancora blu
            Color savedColor = savedCellB2.GetStyle().Font.Color;
            Console.WriteLine("Saved font color: " + savedColor.ToString());
        }
    }
}
```

### Vedi anche

* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


