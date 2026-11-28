---
title: "CellsColor.SetTintOfShapeColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellsColor yöntemi. Şekil renginin tonunu ayarlayın"
type: docs
url: /tr/net/aspose.cells/cellscolor/settintofshapecolor/
---
## CellsColor.SetTintOfShapeColor method

Şekil renginin tonunu ayarla

```csharp
public void SetTintOfShapeColor(double tint)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ton | Double |  |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class CellsColorMethodSetTintOfShapeColorWithDoubleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            try
            {
                // Şeklin dolgu rengini alın
                CellsColor shapeColor = shape.Fill.SolidFill.CellsColor;
                
                // Rengi şekil rengi olarak işlenecek şekilde ayarlayın
                shapeColor.IsShapeColor = true;
                
                // Şekil renginin tonunu ayarlayın (geçerli aralık -1.0 ile 1.0 arasındadır)
                shapeColor.SetTintOfShapeColor(0.5); // Lighten the color by 50%
                
                Console.WriteLine("SetTintOfShapeColor method executed successfully with parameter 0.5");
                
                // Şeklin dolgu rengini değiştirerek efekti gösterin
                shape.Fill.SolidFill.Color = System.Drawing.Color.Blue;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTintOfShapeColor method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("SetTintOfShapeColorWithDoubleDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


