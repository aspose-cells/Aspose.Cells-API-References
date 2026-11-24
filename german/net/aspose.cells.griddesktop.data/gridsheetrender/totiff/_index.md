---
title: "GridSheetRender.ToTiff"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GridSheetRender method. Rendert das gesamte Arbeitsblatt als TIFF‑Bild in einen Stream."
type: docs
url: /de/net/aspose.cells.griddesktop.data/gridsheetrender/totiff/
---
## ToTiff(Stream) {#totiff}

Ganzes Arbeitsblatt als Tiff‑Bild in einen Stream rendern.

```csharp
public void ToTiff(Stream stream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stream | Stream | der Stream des Ausgabebildes |

### Siehe auch

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToTiff(string) {#totiff_1}

Ganzes Arbeitsblatt als Tiff‑Bild in eine Datei rendern.

```csharp
public void ToTiff(string filename)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Dateiname | String | der Dateiname des Ausgabebildes |

### Beispiele

Der folgende Code gibt alle Seiten des ersten Blatts als TIFF‑Bild aus.

```csharp
//Laden Sie die Quelldatei mit Bildern.
Workbook wb = new Workbook("Book1.xlsx");

ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();

//Ausgabetyp des Bildes festlegen.
imgOpt.SaveFormat = SaveFormat.Tiff;

//Das erste Blatt rendern.
SheetRender sr = new SheetRender(wb.Worksheets[0], imgOpt);

//Alle Seiten des Blatts als TIFF‑Bild ausgeben.
sr.ToTiff("output.tiff");
```

### Siehe auch

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


