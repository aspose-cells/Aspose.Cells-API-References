---
title: "GridPdfSaveOptions.SetImageResample"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GridPdfSaveOptions. Imposta i PPI desiderati (pixel per pollice) per le immagini di ricampionamento e la qualità JPEG. Tutte le immagini saranno convertite in JPEG con l'impostazione di qualità specificata e le immagini con una risoluzione superiore ai PPI specificati saranno ricampionate"
type: docs
url: /it/net/aspose.cells.griddesktop.data/gridpdfsaveoptions/setimageresample/
---
## GridPdfSaveOptions.SetImageResample method

Imposta il PPI desiderato (pixel per pollice) per il ridimensionamento delle immagini e la qualità JPEG. Tutte le immagini saranno convertite in JPEG con l'impostazione di qualità specificata, e le immagini che superano il PPI specificato (pixel per pollice) saranno ridimensionate.

```csharp
public void SetImageResample(int desiredPPI, int jpegQuality)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| desiredPPI | Int32 | Pixel per pollice desiderati. 220 alta qualità. 150 qualità schermo. 96 qualità email. |
| jpegQuality | Int32 | 0 - 100% qualità JPEG. |

### Esempi

Il codice seguente imposta i PPI desiderati a 96 e la qualità JPEG a 80 per le immagini nel PDF di output.

```csharp
//carica il file sorgente con le immagini.
Workbook wb = new Workbook("Book1.xlsx");

PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

//imposta i PPI desiderati a 96 e la qualità JPEG a 80.
pdfSaveOptions.SetImageResample(96, 80);

wb.Save("output.pdf", pdfSaveOptions);
```

### Vedi anche

* class [GridPdfSaveOptions](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


