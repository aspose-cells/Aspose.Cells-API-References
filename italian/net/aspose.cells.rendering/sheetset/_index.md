---
title: "Classe SheetSet"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Rendering.SheetSet. Descrive un insieme di fogli"
type: docs
url: /it/net/aspose.cells.rendering/sheetset/
---
## SheetSet class

Descrive un insieme di fogli.

```csharp
public class SheetSet
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [SheetSet](sheetset/#constructor)(params int[]) | Crea un insieme di fogli basato su indici di foglio esatti. |
| [SheetSet](sheetset/#constructor_1)(params string[]) | Crea un insieme di fogli basato su nomi di foglio esatti. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| static [Active](../../aspose.cells.rendering/sheetset/active/) { get; } | Ottiene un insieme con il foglio attivo della cartella di lavoro. |
| static [All](../../aspose.cells.rendering/sheetset/all/) { get; } | Ottiene un insieme con tutti i fogli della cartella di lavoro nel loro ordine originale. |
| static [Visible](../../aspose.cells.rendering/sheetset/visible/) { get; } | Ottiene un insieme con i fogli visibili della cartella di lavoro nel loro ordine originale. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetSetDemo
    {
        public static void SheetSetExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati al worksheet
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(456);   

            worksheet = workbook.Worksheets.Add("test1");
            worksheet.Cells["A1"].PutValue("test Data");
            worksheet.Cells["A2"].PutValue(234);
            worksheet.Cells["A3"].PutValue(333);
            worksheet.IsVisible = false;

            worksheet = workbook.Worksheets.Add("test2");
            worksheet.Cells["A1"].PutValue("test Data222");
            worksheet.Cells["A2"].PutValue(234444);
            worksheet.Cells["A3"].PutValue(333555);

            workbook.Worksheets.ActiveSheetIndex = 0;

            // Crea un oggetto PdfSaveOptions
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // Imposta la proprietà SheetSet per includere solo il foglio attivo
            pdfSaveOptions.SheetSet = SheetSet.Active;

            // Salva la cartella di lavoro in un file PDF
            workbook.Save("SheetSetExample_ActiveSheet.pdf", pdfSaveOptions);

            // Imposta la proprietà SheetSet per includere tutti i fogli visibili
            pdfSaveOptions.SheetSet = SheetSet.Visible;

            // Salva la cartella di lavoro in un file PDF
            workbook.Save("SheetSetExample_VisibleSheets.pdf", pdfSaveOptions);

            // Imposta la proprietà SheetSet per includere tutti i fogli
            pdfSaveOptions.SheetSet = SheetSet.All;

            // Salva la cartella di lavoro in un file PDF
            workbook.Save("SheetSetExample_AllSheets.pdf", pdfSaveOptions);

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


