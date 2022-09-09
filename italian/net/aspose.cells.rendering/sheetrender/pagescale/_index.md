---
title: PageScale
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Ottiene la scala di pagina calcolata del foglio. Restituisce la scala impostata seZoomaspose.cells/pagesetup/zoom è impostato. In caso contrario restituisce la scala calcolata in base aFitToPagesWideaspose.cells/pagesetup/fittopageswide eFitToPagesTallaspose.cells/pagesetup/fittopagestall .
type: docs
weight: 30
url: /it/net/aspose.cells.rendering/sheetrender/pagescale/
---
## SheetRender.PageScale property

Ottiene la scala di pagina calcolata del foglio. Restituisce la scala impostata se[`Zoom`](../../../aspose.cells/pagesetup/zoom) è impostato. In caso contrario, restituisce la scala calcolata in base a[`FitToPagesWide`](../../../aspose.cells/pagesetup/fittopageswide) e[`FitToPagesTall`](../../../aspose.cells/pagesetup/fittopagestall) .

```csharp
public double PageScale { get; }
```

### Esempi

```csharp
Workbook wb = new Workbook("Book1.xlsx");

SheetRender sheetRender = new SheetRender(wb.Worksheets[0], new ImageOrPrintOptions());

//Ottiene la scala di pagina calcolata del foglio.
double pageScale = sheetRender.PageScale;
```

### Guarda anche

* class [SheetRender](../../sheetrender)
* spazio dei nomi [Aspose.Cells.Rendering](../../sheetrender)
* assemblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->