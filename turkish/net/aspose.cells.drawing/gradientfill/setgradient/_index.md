---
title: "GradientFill.SetGradient"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GradientFill yöntemi. Gradyan dolgu tipini ve yönünü ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/gradientfill/setgradient/
---
## GradientFill.SetGradient method

Degrade dolgu türünü ve yönünü ayarlayın.

```csharp
public void SetGradient(GradientFillType type, double angle, GradientDirectionType direction)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | GradientFillType | Gradyan dolgu tipi. |
| angle | Double | Açı. Yalnızca GradientFillType.Linear için geçerlidir. |
| direction | GradientDirectionType | Yön tipi. Yalnızca GradientFillType.Radial ve GradientFillType.Rectangle için geçerlidir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class GradientFillMethodSetGradientWithGradientFillTypeDoubleGradientDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Degrade dolgu uygulamak için bir şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 200, 100);

            try
            {
                // Şeklin dolgu gradyanını al
                GradientFill gradientFill = shape.Fill.GradientFill; // Fixed property name from Gradient to GradientFill
                if (gradientFill == null)
                {
                    Console.WriteLine("Cannot set gradient: The shape's fill is not a GradientFill.");
                    return;
                }

                // SetGradient'i belirli parametrelerle çağır: Doğrusal dolgu, 90 derece, FromCenter yönü
                gradientFill.SetGradient(GradientFillType.Linear, 90.0, GradientDirectionType.FromCenter);
                
                Console.WriteLine("SetGradient method executed successfully with parameters (GradientFillType.Linear, 90.0, GradientDirectionType.FromCenter)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetGradient method: {ex.Message}");
            }
            
            // Etkiyi göstermek için çalışma kitabını kaydedin
            workbook.Save("GradientFillSetGradientDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [GradientFillType](../../gradientfilltype/)
* enum [GradientDirectionType](../../gradientdirectiontype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


