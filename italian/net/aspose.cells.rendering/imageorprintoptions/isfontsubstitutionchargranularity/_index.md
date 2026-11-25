---
title: "ImageOrPrintOptions.IsFontSubstitutionCharGranularity"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageOrPrintOptions. Indica se sostituire solo il carattere del font quando il font della cella non è compatibile con esso"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/isfontsubstitutionchargranularity/
---
## ImageOrPrintOptions.IsFontSubstitutionCharGranularity property

Indica se sostituire solo il font del carattere quando il font della cella non è compatibile.

```csharp
public bool IsFontSubstitutionCharGranularity { get; set; }
```

### Osservazioni

Il valore predefinito è false. Proveremo prima il font predefinito della cartella di lavoro e PdfSaveOption/system per il font della cella.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing; // Added missing namespace AsposeCellsExamples
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyIsFontSubstitutionCharGranularityDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e accedi al primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Configura la cella con un font potenzialmente non supportato
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Text with unavailable font");
            Style style = cell.GetStyle();
            style.Font.Name = "NonExistentFont";
            cell.SetStyle(style);

            // Creare le opzioni di rendering dell'immagine
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Png, // Namespace reference now valid
                DefaultFont = "Arial",
                CheckWorkbookDefaultFont = false
            };

            // Visualizza e modifica il valore della proprietà
            Console.WriteLine($"Initial IsFontSubstitutionCharGranularity: {options.IsFontSubstitutionCharGranularity}");
            
            // Renderizza con l'impostazione predefinita
            new SheetRender(worksheet, options).ToImage(0, "BeforeFontSubstitutionChange.png");

            // Modifica la proprietà e renderizza nuovamente
            options.IsFontSubstitutionCharGranularity = true;
            Console.WriteLine($"Updated IsFontSubstitutionCharGranularity: {options.IsFontSubstitutionCharGranularity}");
            new SheetRender(worksheet, options).ToImage(0, "AfterFontSubstitutionChange.png");

            // Salva la cartella di lavoro per riferimento
            workbook.Save("FontSubstitutionDemoWorkbook.xlsx");
        }
    }
}
```

### Vedi anche

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


