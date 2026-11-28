---
title: "ShapeCollection.AddSpinner"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. Bir Spinner'ı çalışma sayfasına ekler"
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/addspinner/
---
## ShapeCollection.AddSpinner method

Çalışma sayfasına bir Spinner ekler.

```csharp
public Spinner AddSpinner(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| topRow | Int32 | Sol üst satır indeksi. |
| üst | Int32 | Spinner'ın sol satırından dikey ofseti, piksel birimi cinsinden temsil eder. |
| leftColumn | Int32 | Sol üst sütun indeksi. |
| sol | Int32 | Spinner'ın sol sütunundan yatay ofseti, piksel birimi cinsinden temsil eder. |
| yükseklik | Int32 | Spinner'ın yüksekliğini, piksel birimi cinsinden temsil eder. |
| genişlik | Int32 | Spinner'ın genişliğini, piksel birimi cinsinden temsil eder. |

### Dönüş Değeri

Bir Spinner nesnesi.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddSpinnerWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir spinner ekle
            Aspose.Cells.Drawing.Spinner spinner = (Aspose.Cells.Drawing.Spinner)worksheet.Shapes.AddSpinner(1, 0, 1, 0, 100, 50);

            // Spinner özelliklerini ayarla
            spinner.LinkedCell = "A1";
            spinner.Min = 0;
            spinner.Max = 100;
            spinner.IncrementalChange = 1;

            // Çalışma kitabını kaydedin
            workbook.Save("AddSpinnerDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Spinner](../../spinner/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


