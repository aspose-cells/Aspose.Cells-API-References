---
title: "Klass MsoFormatPicture"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.MsoFormatPicture klass. Representerar bildformatet"
type: docs
url: /sv/net/aspose.cells.drawing/msoformatpicture/
---
## MsoFormatPicture class

Representerar bildformatet.

```csharp
public class MsoFormatPicture
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [BottomCrop](../../aspose.cells.drawing/msoformatpicture/bottomcrop/) { get; set; } | Representerar platsen för botten av beskärningsrektangeln, uttryckt som en andel av bildens höjd. |
| [BottomCropInch](../../aspose.cells.drawing/msoformatpicture/bottomcropinch/) { get; set; } | Representerar platsen för den nedre delen av beskärningsrektangeln, uttryckt i tum. |
| [Brightness](../../aspose.cells.drawing/msoformatpicture/brightness/) { get; set; } | Representerar ljusstyrkesmodifieringen för bilden i enhet av procent. |
| [Contrast](../../aspose.cells.drawing/msoformatpicture/contrast/) { get; set; } | Representerar kontrastmodifieringen för bilden.in enhet av procent. |
| [Gamma](../../aspose.cells.drawing/msoformatpicture/gamma/) { get; set; } | Representerar gamma för bilden. |
| [IsBiLevel](../../aspose.cells.drawing/msoformatpicture/isbilevel/) { get; set; } | Indikerar om den här bilden ska visas i tvåfärgs svartvitt. |
| [IsGray](../../aspose.cells.drawing/msoformatpicture/isgray/) { get; set; } | Indikerar om den här bilden ska visas i gråskala. |
| [LeftCrop](../../aspose.cells.drawing/msoformatpicture/leftcrop/) { get; set; } | Representerar platsen för den vänstra sidan av beskärningsrektangeln, uttryckt som en andel av bildens bredd. |
| [LeftCropInch](../../aspose.cells.drawing/msoformatpicture/leftcropinch/) { get; set; } | Representerar platsen för den vänstra sidan av beskärningsrektangeln, uttryckt i tum. |
| [RightCrop](../../aspose.cells.drawing/msoformatpicture/rightcrop/) { get; set; } | Representerar platsen för den högra sidan av beskärningsrektangeln, uttryckt som en andel av bildens bredd. |
| [RightCropInch](../../aspose.cells.drawing/msoformatpicture/rightcropinch/) { get; set; } | Representerar platsen för den högra sidan av beskärningsrektangeln, uttryckt i tum. |
| [TopCrop](../../aspose.cells.drawing/msoformatpicture/topcrop/) { get; set; } | Representerar platsen för den övre delen av beskärningsrektangeln, uttryckt som en andel av bildens höjd. |
| [TopCropInch](../../aspose.cells.drawing/msoformatpicture/topcropinch/) { get; set; } | Representerar platsen för den övre delen av beskärningsrektangeln, uttryckt i tum. |
| [Transparency](../../aspose.cells.drawing/msoformatpicture/transparency/) { get; set; } | Returnerar eller anger graden av transparens för området som ett värde från 0,0 (opak) till 1,0 (klar). |
| [TransparentColor](../../aspose.cells.drawing/msoformatpicture/transparentcolor/) { get; set; } | Hämtar och anger den transparenta färgen för bilden. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/msoformatpicture/equals/)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/msoformatpicture/gethashcode/)() | Hämtar hash‑koden. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till en bild i arbetsbladet
            int pictureIndex = sheet.Pictures.Add(5, 5, "MsoFormatPictureDemo.jpg");
            Picture picture = sheet.Pictures[pictureIndex];

            // Åtkomst till MsoFormatPicture‑objektet
            MsoFormatPicture formatPicture = picture.FormatPicture;

            // Ställ in egenskaper för MsoFormatPicture
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

            // Ange den transparenta färgen
            CellsColor transparentColor = workbook.CreateCellsColor();
            transparentColor.Color = Color.White;
            formatPicture.TransparentColor = transparentColor;

            // Spara arbetsboken
            workbook.Save("MsoFormatPictureDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


