---
title: "BackgroundType enum"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.BackgroundType enum. Hücre arka planı desen türlerini sıralar"
type: docs
url: /tr/net/aspose.cells/backgroundtype/
---
## BackgroundType enumeration

Hücre arka plan desen türlerini listeler.

```csharp
public enum BackgroundType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| DiagonalCrosshatch | `9` | Diyagonal çapraz çizgi desenini temsil eder. |
| DiagonalStripe | `8` | Diyagonal şerit desenini temsil eder. |
| Gray6 | `18` | %6,25 gri desenini temsil eder |
| Gray12 | `17` | %12,5 gri desenini temsil eder |
| Gray25 | `4` | %25 gri desenini temsil eder. |
| Gray50 | `2` | %50 gri desenini temsil eder. |
| Gray75 | `3` | %75 gri desenini temsil eder. |
| HorizontalStripe | `5` | Yatay şerit desenini temsil eder. |
| None | `0` | Arka plan yoktur. |
| ReverseDiagonalStripe | `7` | Ters diyagonal şerit desenini temsil eder. |
| Solid | `1` | Düz desenini temsil eder. |
| ThickDiagonalCrosshatch | `10` | Kalın diyagonal çapraz çizgi desenini temsil eder. |
| ThinDiagonalCrosshatch | `16` | İnce diyagonal çapraz çizgi desenini temsil eder. |
| ThinDiagonalStripe | `14` | İnce diyagonal şerit desenini temsil eder. |
| ThinHorizontalCrosshatch | `15` | İnce yatay çapraz çizgi desenini temsil eder. |
| ThinHorizontalStripe | `11` | İnce yatay şerit desenini temsil eder. |
| ThinReverseDiagonalStripe | `13` | İnce ters diyagonal şerit desenini temsil eder. |
| ThinVerticalStripe | `12` | İnce dikey şerit desenini temsil eder. |
| VerticalStripe | `6` | Dikey şerit desenini temsil eder. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class BackgroundTypeDemo
    {
        public static void BackgroundTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Çalışma kitabındaki ilk çalışma sayfasına erişin
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasından bir hücreye erişin
            Cell cell = worksheet.Cells["A1"];
            
            // Hücrenin değerini ayarlayın
            cell.PutValue("Hello, Aspose!");

            // Bir stil nesnesi oluşturun
            Style style = cell.GetStyle();
            
            // Arka plan desen tipini ayarlayın
            style.Pattern = BackgroundType.DiagonalStripe;
            
            // Ön plan rengini ayarlayın
            style.ForegroundColor = Color.Red;
            
            // Arka plan rengini ayarlayın
            style.BackgroundColor = Color.Green;
            
            // Stili hücreye uygulayın
            cell.SetStyle(style);
            
            // Çalışma kitabını kaydedin
            workbook.Save("BackgroundTypeExample.xlsx");
            workbook.Save("BackgroundTypeExample.pdf");



        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


