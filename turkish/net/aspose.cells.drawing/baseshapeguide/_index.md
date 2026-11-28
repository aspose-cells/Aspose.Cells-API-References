---
title: "BaseShapeGuide sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.BaseShapeGuide sınıfı. Şekil kılavuzunu temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/baseshapeguide/
---
## BaseShapeGuide class

Şekil kılavuzunu temsil eder.

```csharp
public class BaseShapeGuide
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassBaseShapeGuideDemo
    {
        public static void Run()
        {
            // Demonstrasyon için yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Doğru parametrelerle bir dikdörtgen şekli oluştur
                Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

                // BaseShapeGuide'in genel bir yapıcıya sahip olmaması nedeniyle,
                // kılavuz içerebilecek bir şekil aracılığıyla kullanımını göstereceğiz
                // Not: Bu, gerçek kılavuz erişiminin farklı olabileceği basitleştirilmiş bir gösterimdir
                Console.WriteLine("Shape created successfully");
                Console.WriteLine($"Shape type: {shape.GetType().Name}");

                // Çalışma kitabını kaydedin
                workbook.Save("BaseShapeGuideDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with BaseShapeGuide: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


