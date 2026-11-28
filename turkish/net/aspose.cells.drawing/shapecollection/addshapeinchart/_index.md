---
title: "ShapeCollection.AddShapeInChart"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. Çart'a bir şekil ekle. Tüm birim çart alanının 1/4000'idir."
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/addshapeinchart/
---
## AddShapeInChart(MsoDrawingType, PlacementType, int, int, int, int, byte[]) {#addshapeinchart_1}

Grafiğe bir şekil ekle. Tüm birim, grafik alanının 1/4000'idir.

```csharp
public Shape AddShapeInChart(MsoDrawingType type, PlacementType placement, int left, int top, 
    int right, int bottom, byte[] imageData)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | MsoDrawingType | Çizim türü. |
| yerleştirme | PlacementType | yerleştirme türü. |
| sol | Int32 | Çart alanı genişliğinin 1/4000 biriminde. |
| üst | Int32 | Çart alanı yüksekliğinin 1/4000 biriminde. |
| sağ | Int32 | Çart alanı genişliğinin 1/4000 biriminde. |
| alt | Int32 | Çart alanı yüksekliğinin 1/4000 biriminde. |
| imageData | Byte[] | Şekil bir resim veya ole nesnesi değilse, imageData null olmalıdır. |

### Ayrıca Bakınız

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* enum [PlacementType](../../placementtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## AddShapeInChart(MsoDrawingType, PlacementType, int, int, int, int) {#addshapeinchart}

Grafiğe bir şekil ekle. Tüm birim, grafik alanının 1/4000'idir.

```csharp
public Shape AddShapeInChart(MsoDrawingType type, PlacementType placement, int left, int top, 
    int right, int bottom)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | MsoDrawingType | Çizim türü. |
| yerleştirme | PlacementType | yerleştirme türü. |
| sol | Int32 | Çart alanı genişliğinin 1/4000 biriminde. |
| üst | Int32 | Çart alanı yüksekliğinin 1/4000 biriminde. |
| sağ | Int32 | Çart alanı genişliğinin 1/4000 biriminde. |
| alt | Int32 | Çart alanı yüksekliğinin 1/4000 biriminde. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddShapeInChartWithMsoDrawingTypePlacementTypeIntDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Şekli çarta ekle
            chart.Shapes.AddShapeInChart(MsoDrawingType.CheckBox, PlacementType.Move, 100, 100, 1000, 1000);
            
            // Şekil metnini ayarla
            chart.Shapes[0].Text = "Sample CheckBox";
            
            // Çalışma kitabını kaydet
            workbook.Save("AddShapeInChartWithMsoDrawingType.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* enum [PlacementType](../../placementtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


