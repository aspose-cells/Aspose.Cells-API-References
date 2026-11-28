---
title: "ShapePropertyCollection.HasGlowEffect"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapePropertyCollection yöntemi. Şeklin parlama efekti verisini gösterir"
type: docs
url: /tr/net/aspose.cells.drawing/shapepropertycollection/hasgloweffect/
---
## ShapePropertyCollection.HasGlowEffect method

Şeklin parıltı etkisi verisine sahip olup olmadığını gösterir.

```csharp
public bool HasGlowEffect()
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;
    using System;

    public class ShapePropertyCollectionMethodHasGlowEffectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek bir grafik oluşturun
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);

            chart.NSeries.Add("B1:B2", true);
            chart.NSeries.CategoryData = "A1:A2";

            // İlk serinin şekil özelliklerine erişin
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            ShapePropertyCollection shapeProperties = series.ShapeProperties;

            // 3B biçimi ve köşe yuvarlamasını yapılandırın
            Format3D format3D = shapeProperties.Format3D;
            Bevel topBevel = format3D.TopBevel;

            topBevel.Type = BevelPresetType.Circle;
            topBevel.Height = 2;
            topBevel.Width = 5;

            format3D.SurfaceMaterialType = PresetMaterialType.WarmMatte;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;
            format3D.LightingAngle = 20;

            GlowEffect glowEffect = shapeProperties.GlowEffect;
            glowEffect.Size = 30;
            glowEffect.Color.Color = Color.Red;

            Console.WriteLine("Shape has glow effect: " + shapeProperties.HasGlowEffect());
                       

            // Sonucu kaydet
            workbook.Save("ShapePropertyCollectionMethodHasGlowEffectDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ShapePropertyCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


