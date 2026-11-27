---
title: "GridSheetRender.ToTiff"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridSheetRender metod. Renderar hela arbetsbladet som en Tiff‑bild till en ström"
type: docs
url: /sv/net/aspose.cells.griddesktop.data/gridsheetrender/totiff/
---
## ToTiff(Stream) {#totiff}

Rendera hela kalkylbladet som Tiff Image till en ström.

```csharp
public void ToTiff(Stream stream)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | Ström | strömmen för den utgående bilden |

### Se även

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToTiff(string) {#totiff_1}

Rendera hela kalkylbladet som Tiff Image till en fil.

```csharp
public void ToTiff(string filename)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filnamn | String | filnamnet för den utgående bilden |

### Exempel

Följande kod skriver ut alla sidor i det första bladet till en Tiff‑bild.

```csharp
//läs in källfilen med bilder.
Workbook wb = new Workbook("Book1.xlsx");

ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();

//ange output‑bildtyp.
imgOpt.SaveFormat = SaveFormat.Tiff;

//rendera det första bladet.
SheetRender sr = new SheetRender(wb.Worksheets[0], imgOpt);

//exportera alla sidor i bladet till en Tiff-bild.
sr.ToTiff("output.tiff");
```

### Se även

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


