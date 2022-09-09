---
title: EvaluatedPageCount
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Valuta il conteggio totale delle pagine di questo foglio di lavoro
type: docs
weight: 20
url: /it/net/aspose.cells.rendering/sheetprintingpreview/evaluatedpagecount/
---
## SheetPrintingPreview.EvaluatedPageCount property

Valuta il conteggio totale delle pagine di questo foglio di lavoro

```csharp
public int EvaluatedPageCount { get; }
```

### Esempi

Il codice seguente mostra il modo più veloce per ottenere il conteggio delle pagine di un foglio di lavoro.

```csharp
Workbook workbook = new Workbook("Book1.xlsx");

SheetPrintingPreview sheetPrintingPreview = new SheetPrintingPreview(workbook.Worksheets[0], new ImageOrPrintOptions());

//il modo più veloce per ottenere il conteggio delle pagine specialmente quando ci sono dati enormi nel foglio di lavoro.
Console.WriteLine(sheetPrintingPreview.EvaluatedPageCount);
        
```

### Guarda anche

* class [SheetPrintingPreview](../../sheetprintingpreview)
* spazio dei nomi [Aspose.Cells.Rendering](../../sheetprintingpreview)
* assemblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->