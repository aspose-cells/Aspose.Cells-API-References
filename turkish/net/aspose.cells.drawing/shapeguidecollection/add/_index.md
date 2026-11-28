---
title: "ShapeGuideCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeGuideCollection yöntemi. Bir şekil kılavuzu ekler. Önemli: Bu özellik şu anda yalnızca Excel07 ve üzeri için kullanılabilir"
type: docs
url: /tr/net/aspose.cells.drawing/shapeguidecollection/add/
---
## ShapeGuideCollection.Add method

Bir şekil kılavuzu ekler. (Önemli: Bu özellik şu anda yalnızca Excel07 ve üzeri için mevcuttur)

```csharp
public int Add(string name, double val)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | ayarın adı. "adj (Yalnızca bir ayarlama değeri olduğunda kullanılır)", "adj1", "adj2", "adj3" vb. şeklindedir. |
| val | Double | ayarın değeri |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeGuideCollectionMethodAddWithStringDoubleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasına erişin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ayar kılavuzlarını kullanan bir şekil oluştur
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.RightArrowCallout, 2, 0, 2, 0, 200, 150);

            try
            {
                // Şekil geometrisi ayarlamalarından ShapeGuideCollection'ı al
                ShapeGuideCollection shapeGuides = shape.Geometry.ShapeAdjustValues;

                // (String, Double) parametreleriyle Add metodunu çağır
                shapeGuides.Add("adj1", 25.5);
                shapeGuides.Add("adj2", 25.5);
                shapeGuides.Add("adj3", 25.5);
                shapeGuides.Add("adj4", 25.5);

                Console.WriteLine($"Total guides after addition: {shapeGuides.Count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }

            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("ShapeGuideAddWithStringDoubleDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ShapeGuideCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


