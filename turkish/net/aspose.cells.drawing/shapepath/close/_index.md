---
title: "ShapePath.Close"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapePath yöntemi. Mevcut şekli kapatır ve yeni bir şekil başlatır. Mevcut şekil bir dizi bağlı çizgi ve eğri içeriyorsa, yöntem son noktayı başlangıç noktasına bir çizgiyle bağlayarak döngüyü kapatır."
type: docs
url: /tr/net/aspose.cells.drawing/shapepath/close/
---
## ShapePath.Close method

Mevcut şekli kapatır ve yeni bir şekil başlatır. Mevcut şekil bağlı çizgiler ve eğrilerden oluşan bir dizi içeriyorsa, yöntem son noktayı başlangıç noktasına bir çizgiyle bağlayarak döngüyü kapatır.

```csharp
public void Close()
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodCloseDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                //Yeni bir şekil yolu oluştur
                ShapePath shapePath = new ShapePath();
                shapePath.MoveTo(60, 45);
                shapePath.ArcTo(25, 25, 0, 270);

                // Yolu kapat 
                shapePath.Close();

                shapePath.MoveTo(60, 20);
                shapePath.LineTo(110, 70);
                shapePath.LineTo(125, 155.5f);
                shapePath.ArcTo(35.5f, 35.5f, 0, 270);

                // Yolu kapat 
                shapePath.Close();

                //serbest form ekle
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath });

                Console.WriteLine("Close method called successfully to complete the shape path");
                
                // Çalışma kitabını kaydedin
                workbook.Save("ShapePathMethodCloseDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling Close method: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


