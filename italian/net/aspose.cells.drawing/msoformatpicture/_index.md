---
title: "Classe MsoFormatPicture"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.MsoFormatPicture classe. Rappresenta il formato dell'immagine"
type: docs
url: /it/net/aspose.cells.drawing/msoformatpicture/
---
## MsoFormatPicture class

Rappresenta il formato immagine.

```csharp
public class MsoFormatPicture
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BottomCrop](../../aspose.cells.drawing/msoformatpicture/bottomcrop/) { get; set; } | Rappresenta la posizione del bordo inferiore del rettangolo di ritaglio, espressa come rapporto rispetto all'altezza dell'immagine. |
| [BottomCropInch](../../aspose.cells.drawing/msoformatpicture/bottomcropinch/) { get; set; } | Rappresenta la posizione del bordo inferiore del rettangolo di ritaglio, in unità di pollici. |
| [Brightness](../../aspose.cells.drawing/msoformatpicture/brightness/) { get; set; } | Rappresenta la modifica della luminosità dell'immagine in unità di percentuale. |
| [Contrast](../../aspose.cells.drawing/msoformatpicture/contrast/) { get; set; } | Rappresenta la modifica del contrasto dell'immagine in unità di percentuale. |
| [Gamma](../../aspose.cells.drawing/msoformatpicture/gamma/) { get; set; } | Rappresenta la gamma dell'immagine. |
| [IsBiLevel](../../aspose.cells.drawing/msoformatpicture/isbilevel/) { get; set; } | Indica se questa immagine deve essere visualizzata in bianco e nero a due colori. |
| [IsGray](../../aspose.cells.drawing/msoformatpicture/isgray/) { get; set; } | Indica se questa immagine deve essere visualizzata in scala di grigi. |
| [LeftCrop](../../aspose.cells.drawing/msoformatpicture/leftcrop/) { get; set; } | Rappresenta la posizione del bordo sinistro del rettangolo di ritaglio, espressa come rapporto rispetto alla larghezza dell'immagine. |
| [LeftCropInch](../../aspose.cells.drawing/msoformatpicture/leftcropinch/) { get; set; } | Rappresenta la posizione del bordo sinistro del rettangolo di ritaglio, in unità di pollici. |
| [RightCrop](../../aspose.cells.drawing/msoformatpicture/rightcrop/) { get; set; } | Rappresenta la posizione del bordo destro del rettangolo di ritaglio, espressa come rapporto rispetto alla larghezza dell'immagine. |
| [RightCropInch](../../aspose.cells.drawing/msoformatpicture/rightcropinch/) { get; set; } | Rappresenta la posizione del bordo destro del rettangolo di ritaglio, in unità di pollici. |
| [TopCrop](../../aspose.cells.drawing/msoformatpicture/topcrop/) { get; set; } | Rappresenta la posizione del bordo superiore del rettangolo di ritaglio, espressa come rapporto rispetto all'altezza dell'immagine. |
| [TopCropInch](../../aspose.cells.drawing/msoformatpicture/topcropinch/) { get; set; } | Rappresenta la posizione del bordo superiore del rettangolo di ritaglio, in unità di pollici. |
| [Transparency](../../aspose.cells.drawing/msoformatpicture/transparency/) { get; set; } | Restituisce o imposta il grado di trasparenza dell'area come valore da 0,0 (opaco) a 1,0 (trasparente). |
| [TransparentColor](../../aspose.cells.drawing/msoformatpicture/transparentcolor/) { get; set; } | Ottiene e imposta il colore trasparente dell'immagine. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/msoformatpicture/equals/)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/msoformatpicture/gethashcode/)() | Ottiene il codice hash. |

### Esempi

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPictureDemo
    {
        public static void RunDemo()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi un'immagine al foglio di lavoro
            int pictureIndex = sheet.Pictures.Add(5, 5, "MsoFormatPictureDemo.jpg");
            Picture picture = sheet.Pictures[pictureIndex];

            // Accedi all'oggetto MsoFormatPicture
            MsoFormatPicture formatPicture = picture.FormatPicture;

            // Imposta le proprietà di MsoFormatPicture
            formatPicture.TopCropInch = 0.5;
            formatPicture.BottomCropInch = 0.5;
            formatPicture.LeftCropInch = 0.5;
            formatPicture.RightCropInch = 0.5;
            formatPicture.Transparency = 0.5;
            formatPicture.Contrast = 0.8;
            formatPicture.Brightness = 0.6;
            formatPicture.Gamma = 1.0;
            formatPicture.IsBiLevel = false;
            formatPicture.IsGray = false;

            // Imposta il colore trasparente
            CellsColor transparentColor = workbook.CreateCellsColor();
            transparentColor.Color = Color.White;
            formatPicture.TransparentColor = transparentColor;

            // Salva la cartella di lavoro
            workbook.Save("MsoFormatPictureDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


