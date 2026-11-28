---
title: "ShapeCollection.AddTextEffectInChart"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. Grafik içine bir WordArt nesnesi ekler."
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/addtexteffectinchart/
---
## ShapeCollection.AddTextEffectInChart method

Grafiğe bir WordArt nesnesi ekler.

```csharp
public Shape AddTextEffectInChart(MsoPresetTextEffect effect, string text, string fontName, 
    int size, bool fontBold, bool fontItalic, int top, int left, int height, int width)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| efekt | MsoPresetTextEffect | mso ön ayarlı metin efekti türü. |
| metin | String | WordArt metni. |
| fontName | String | Yazı tipi adı. |
| boyut | Int32 | Yazı tipi boyutu |
| fontBold | Boolean | Yazı tipinin kalın olup olmadığını gösterir. |
| fontItalic | Boolean | Yazı tipinin italik olup olmadığını gösterir. |
| üst | Int32 | Şeklin sol üst köşeden dikey ofsetini, grafik alanının 1/4000 birimi cinsinden temsil eder. |
| sol | Int32 | Şeklin sol üst köşeden dikey ofsetini, grafik alanının 1/4000 birimi cinsinden temsil eder. |
| yükseklik | Int32 | Şeklin yüksekliğini, grafik alanının 1/4000 birimi cinsinden temsil eder. |
| genişlik | Int32 | Şeklin genişliğini, grafik alanının 1/4000 birimi cinsinden temsil eder. |

### Dönüş Değeri

Yeni WordArt nesnesini temsil eden bir Shape nesnesi döndürür.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddTextEffectInChartWithMsoPresetTextEffectStringStrinDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş ve örnek veri ekle
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            
            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);
            
            // Grafiğe WordArt ekle
            Shape wordart = chart.Shapes.AddTextEffectInChart(
                MsoPresetTextEffect.TextEffect2,
                "SAMPLE TEXT", 
                "Arial Black", 
                36, 
                false, 
                false,
                100,  // Left position
                100,  // Top position
                300,  // Width
                200); // Height
                
            // WordArt görünümünü özelleştir
            wordart.FillFormat.Transparency = 0.7;
            wordart.LineFormat.IsVisible = false;
            
            // Çalışma kitabını kaydedin
            workbook.Save("WordArtInChart.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../../shape/)
* enum [MsoPresetTextEffect](../../msopresettexteffect/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


