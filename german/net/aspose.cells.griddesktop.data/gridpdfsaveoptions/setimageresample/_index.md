---
title: "GridPdfSaveOptions.SetImageResample"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GridPdfSaveOptions-Methode. Legt die gewünschte PPI (Pixel pro Zoll) für das Resamplen von Bildern und die JPEG-Qualität fest. Alle Bilder werden in JPEG mit der angegebenen Qualitätseinstellung konvertiert, und Bilder, die größer als die angegebene PPI (Pixel pro Zoll) sind, werden resampelt."
type: docs
url: /de/net/aspose.cells.griddesktop.data/gridpdfsaveoptions/setimageresample/
---
## GridPdfSaveOptions.SetImageResample method

Setzt die gewünschte PPI (Pixel pro Zoll) für das Resampling von Bildern und die JPEG‑Qualität. Alle Bilder werden mit der angegebenen Qualitätseinstellung in JPEG konvertiert, und Bilder, die größer als die angegebene PPI (Pixel pro Zoll) sind, werden neu gesampelt.

```csharp
public void SetImageResample(int desiredPPI, int jpegQuality)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| desiredPPI | Int32 | Gewünschte Pixel pro Zoll. 220 hohe Qualität. 150 Bildschirmqualität. 96 E-Mail-Qualität. |
| jpegQuality | Int32 | 0 - 100 % JPEG‑Qualität. |

### Beispiele

Der folgende Code setzt die gewünschte PPI auf 96 und die JPEG-Qualität auf 80 für Bilder im Ausgabe-PDF.

```csharp
//Laden Sie die Quelldatei mit Bildern.
Workbook wb = new Workbook("Book1.xlsx");

PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

//Setzen Sie die gewünschte PPI auf 96 und die JPEG-Qualität auf 80.
pdfSaveOptions.SetImageResample(96, 80);

wb.Save("output.pdf", pdfSaveOptions);
```

### Siehe auch

* class [GridPdfSaveOptions](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


