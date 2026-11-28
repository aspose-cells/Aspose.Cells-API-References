---
title: "Sınıf SolidFill"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.SolidFill sınıfı. Katı dolgu biçimini temsil eden nesneyi kapsüller"
type: docs
url: /tr/net/aspose.cells.drawing/solidfill/
---
## SolidFill class

Katı dolgu biçimini temsil eden nesneyi kapsüller

```csharp
public class SolidFill : Fill
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CellsColor](../../aspose.cells.drawing/solidfill/cellscolor/) { get; set; } | Alır ve ayarlar [`CellsColor`](./cellscolor/) nesnesini. |
| [Color](../../aspose.cells.drawing/solidfill/color/) { get; set; } | Alır veya ayarlar Rengi. |
| [Transparency](../../aspose.cells.drawing/solidfill/transparency/) { get; set; } | Alan şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak döndürür veya ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/solidfill/equals/)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/solidfill/gethashcode/)() | Hash kodunu alır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using System;
    using System.Drawing;
    using Aspose.Cells;
    using Aspose.Cells.Drawing;

    public class DrawingClassSolidFillDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasını alın.
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            try
            {
                // Sayfaya basit bir dikdörtgen şekli ekle
                Shape rect = sheet.Shapes.AddRectangle(2, 0, 2, 0, 150, 100);

                // Şekli katı dolgu kullanacak şekilde yapılandır
                rect.Fill.FillType = FillType.Solid;

                // SolidFill nesnesini elde et
                SolidFill solidFill = rect.Fill.SolidFill;

                // Katı dolgu özelliklerini ayarla
                solidFill.Color = Color.CornflowerBlue;   // System.Drawing.Color
                solidFill.Transparency = 0.25;            // 0 = opaque, 1 = fully transparent

                // CellsColor özelliğine erişin (okuma/yazma)
                CellsColor cellsColor = solidFill.CellsColor;
                if (cellsColor != null)
                {
                    Console.WriteLine("CellsColor object is available.");
                }
                else
                {
                    Console.WriteLine("CellsColor is null (default).");
                }

                Console.WriteLine($"SolidFill created with Color={solidFill.Color.Name}, Transparency={solidFill.Transparency}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SolidFill: {ex.Message}");
            }

            // Şeklin görünümünü doğrulamak için çalışma kitabını kaydedin
            workbook.Save("DrawingClassSolidFillDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


