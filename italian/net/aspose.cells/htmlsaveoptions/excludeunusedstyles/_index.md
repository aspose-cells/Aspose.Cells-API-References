---
title: "HtmlSaveOptions.ExcludeUnusedStyles"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se escludere gli stili non utilizzati. Per i file HTML generati, l'esclusione degli stili inutilizzati può ridurre la dimensione del file senza influire sugli effetti visivi. Pertanto, il valore predefinito di questa proprietà è true. Se l'utente ha bisogno di mantenere tutti gli stili nel workbook per l'HTML generato, ad esempio nello scenario in cui l'utente deve ripristinare il workbook dall'HTML generato in seguito, si prega di impostare questa proprietà su false."
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/excludeunusedstyles/
---
## HtmlSaveOptions.ExcludeUnusedStyles property

Indica se escludere gli stili non utilizzati. Per i file html generati, escludere gli stili non utilizzati può ridurre la dimensione del file senza influire sugli effetti visivi. Pertanto il valore predefinito di questa proprietà è true. Se l'utente deve mantenere tutti gli stili nella cartella di lavoro per l'html generato (ad esempio nello scenario in cui l'utente deve ripristinare la cartella di lavoro dall'html generato in seguito), impostare questa proprietà su false.

```csharp
public bool ExcludeUnusedStyles { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExcludeUnusedStylesDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Aggiungi dati di esempio con stili diversi
            Cell cell1 = workbook.Worksheets[0].Cells["A1"];
            cell1.Value = "Styled text";
            Style style1 = cell1.GetStyle();
            style1.Font.Color = Color.Red;
            style1.Font.IsBold = true;
            cell1.SetStyle(style1);

            Cell cell2 = workbook.Worksheets[0].Cells["A2"];
            cell2.Value = "Different style";
            Style style2 = cell2.GetStyle();
            style2.Font.Name = "Times New Roman";
            style2.Font.Size = 14;
            cell2.SetStyle(style2);

            // Configura le opzioni di salvataggio HTML per escludere gli stili non utilizzati
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExcludeUnusedStyles = true;

            // Salva la cartella di lavoro con le opzioni HTML
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);

            Console.WriteLine("HTML file saved with ExcludeUnusedStyles=true");
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


