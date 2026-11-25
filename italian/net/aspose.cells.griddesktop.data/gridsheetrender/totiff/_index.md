---
title: "GridSheetRender.ToTiff"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "GridSheetRender method. Renderizza l'intero foglio di lavoro come immagine Tiff nello stream"
type: docs
url: /it/net/aspose.cells.griddesktop.data/gridsheetrender/totiff/
---
## ToTiff(Stream) {#totiff}

Renderizza l'intero foglio di lavoro come immagine Tiff nello stream.

```csharp
public void ToTiff(Stream stream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream | lo stream dell'immagine di output |

### Vedi anche

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToTiff(string) {#totiff_1}

Renderizza l'intero foglio di lavoro come immagine Tiff in un file.

```csharp
public void ToTiff(string filename)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filename | String | il nome file dell'immagine di output |

### Esempi

Il codice seguente genera tutte le pagine del primo foglio in immagine Tiff.

```csharp
//carica il file sorgente con le immagini.
Workbook wb = new Workbook("Book1.xlsx");

ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();

//Imposta il tipo di immagine di output.
imgOpt.SaveFormat = SaveFormat.Tiff;

//Renderizza il primo foglio.
SheetRender sr = new SheetRender(wb.Worksheets[0], imgOpt);

//Esporta tutte le pagine del foglio in immagine Tiff.
sr.ToTiff("output.tiff");
```

### Vedi anche

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


