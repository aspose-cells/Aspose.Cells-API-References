---
title: "Class MsoFormatPicture"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.MsoFormatPicture sınıfı. Resim formatını temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/msoformatpicture/
---
## MsoFormatPicture class

Resim biçimini temsil eder.

```csharp
public class MsoFormatPicture
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [BottomCrop](../../aspose.cells.drawing/msoformatpicture/bottomcrop/) { get; set; } | Kırpma dikdörtgeninin alt konumunu, görüntünün yüksekliğine oran olarak ifade eder. |
| [BottomCropInch](../../aspose.cells.drawing/msoformatpicture/bottomcropinch/) { get; set; } | Kırpma dikdörtgeninin alt konumunu, inç cinsinden ifade eder. |
| [Brightness](../../aspose.cells.drawing/msoformatpicture/brightness/) { get; set; } | Resmin parlaklık değişimini yüzde biriminde temsil eder. |
| [Contrast](../../aspose.cells.drawing/msoformatpicture/contrast/) { get; set; } | Resmin kontrast değişimini yüzde biriminde temsil eder. |
| [Gamma](../../aspose.cells.drawing/msoformatpicture/gamma/) { get; set; } | Resmin gamasını temsil eder. |
| [IsBiLevel](../../aspose.cells.drawing/msoformatpicture/isbilevel/) { get; set; } | Bu resmin iki renkli siyah-beyaz olarak görüntülenip görüntülenmeyeceğini gösterir. |
| [IsGray](../../aspose.cells.drawing/msoformatpicture/isgray/) { get; set; } | Bu resmin gri tonlamada görüntülenip görüntülenmeyeceğini gösterir. |
| [LeftCrop](../../aspose.cells.drawing/msoformatpicture/leftcrop/) { get; set; } | Kırpma dikdörtgeninin sol konumunu, görüntünün genişliğine oran olarak ifade eder. |
| [LeftCropInch](../../aspose.cells.drawing/msoformatpicture/leftcropinch/) { get; set; } | Kırpma dikdörtgeninin sol konumunu, inç cinsinden ifade eder. |
| [RightCrop](../../aspose.cells.drawing/msoformatpicture/rightcrop/) { get; set; } | Kırpma dikdörtgeninin sağ konumunu, görüntünün genişliğine oran olarak ifade eder. |
| [RightCropInch](../../aspose.cells.drawing/msoformatpicture/rightcropinch/) { get; set; } | Kırpma dikdörtgeninin sağ konumunu, inç cinsinden ifade eder. |
| [TopCrop](../../aspose.cells.drawing/msoformatpicture/topcrop/) { get; set; } | Kırpma dikdörtgeninin üst konumunu, görüntünün yüksekliğine oran olarak ifade eder. |
| [TopCropInch](../../aspose.cells.drawing/msoformatpicture/topcropinch/) { get; set; } | Kırpma dikdörtgeninin üst konumunu, inç cinsinden ifade eder. |
| [Transparency](../../aspose.cells.drawing/msoformatpicture/transparency/) { get; set; } | Alan şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak döndürür veya ayarlar. |
| [TransparentColor](../../aspose.cells.drawing/msoformatpicture/transparentcolor/) { get; set; } | Resmin şeffaf rengini alır ve ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/msoformatpicture/equals/)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/msoformatpicture/gethashcode/)() | Hash kodunu alır. |

### Örnekler

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
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir resim ekle
            int pictureIndex = sheet.Pictures.Add(5, 5, "MsoFormatPictureDemo.jpg");
            Picture picture = sheet.Pictures[pictureIndex];

            // MsoFormatPicture nesnesine erişin
            MsoFormatPicture formatPicture = picture.FormatPicture;

            // MsoFormatPicture özelliklerini ayarlayın
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

            // Şeffaf rengi ayarlayın
            CellsColor transparentColor = workbook.CreateCellsColor();
            transparentColor.Color = Color.White;
            formatPicture.TransparentColor = transparentColor;

            // Çalışma kitabını kaydedin
            workbook.Save("MsoFormatPictureDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


