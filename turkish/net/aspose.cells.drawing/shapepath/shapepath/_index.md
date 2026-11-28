---
title: "ShapePath.ShapePath"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapePath yapıcı. ShapePath sınıfının yeni bir örneğini başlatır"
type: docs
url: /tr/net/aspose.cells.drawing/shapepath/shapepath/
---
## ShapePath constructor

[`ShapePath`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public ShapePath()
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodCtorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // #ctor yöntemini kullanarak yeni bir şekil yolu oluşturun
                ShapePath shapePath = new ShapePath();

                // Basit bir şekil oluşturmak için yol segmentleri ekleyin
                shapePath.MoveTo(100, 100);
                shapePath.LineTo(200, 100);
                shapePath.LineTo(200, 200);
                shapePath.LineTo(100, 200);
                shapePath.Close();

                //serbest form ekle
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 200, 200, new ShapePath[] { shapePath });

                Console.WriteLine("ShapePath created and added to worksheet successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ShapePath constructor: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("ShapePathMethodCtorDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


