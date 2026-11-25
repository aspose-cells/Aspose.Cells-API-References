---
title: "HtmlSaveOptions.SheetSet"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Ottiene o imposta i fogli da renderizzare. Il valore predefinito è tutti i fogli visibili nella cartella di lavoro (Visible)."
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/sheetset/
---
## HtmlSaveOptions.SheetSet property

Ottiene o imposta i fogli da renderizzare. Il valore predefinito è tutti i fogli visibili nella cartella di lavoro: [`Visible`](../../../aspose.cells.rendering/sheetset/visible/).

```csharp
public SheetSet SheetSet { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class HtmlSaveOptionsPropertySheetSetDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro con più fogli di lavoro
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");
            
            // Rendi un foglio nascosto per la dimostrazione
            workbook.Worksheets[1].IsVisible = false;

            // Imposta alcuni dati di esempio in ogni foglio
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Worksheet sheet = workbook.Worksheets[i];
                sheet.Cells["A1"].PutValue($"Data from {sheet.Name}");
            }

            // Crea un'istanza di HtmlSaveOptions
            HtmlSaveOptions options = new HtmlSaveOptions();

            // Visualizza il valore corrente di SheetSet (il valore predefinito è null, che significa tutti i fogli visibili)
            Console.WriteLine("Current SheetSet value: " + (options.SheetSet == null ? "All visible sheets" : "Custom set"));

            // Imposta SheetSet per includere solo fogli specifici (per indice)
            options.SheetSet = new SheetSet(new int[] { 0, 2 });

            // Salva in HTML - saranno inclusi solo i fogli specificati
            workbook.Save("HtmlWithCustomSheetSet.html", options);

            // Modifica SheetSet per includere solo i fogli visibili
            options.SheetSet = SheetSet.Visible;
            workbook.Save("HtmlWithVisibleSheets.html", options);

            // Modifica SheetSet per includere solo il foglio attivo
            workbook.Worksheets[2].IsSelected = true; // Activate the sheet by selecting it
            options.SheetSet = SheetSet.Active;
            workbook.Save("HtmlWithActiveSheet.html", options);
        }
    }
}
```

### Vedi anche

* class [SheetSet](../../../aspose.cells.rendering/sheetset/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


