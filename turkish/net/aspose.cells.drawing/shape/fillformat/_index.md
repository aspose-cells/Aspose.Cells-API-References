---
title: "Shape.FillFormat"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Şekil özelliği. Belirtilen şekil için dolgu biçimlendirme özelliklerini içeren bir MsoFillFormat nesnesi döndürür"
type: docs
url: /tr/net/aspose.cells.drawing/shape/fillformat/
---
## Shape.FillFormat property

Belirtilen şekil için dolgu biçimlendirme özelliklerini içeren bir MsoFillFormat nesnesi döndürür.

```csharp
[Obsolete("Use Shape.Fill property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MsoFillFormat FillFormat { get; }
```

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Shape.Fill özelliğini kullanın. Bu özellik Temmuz 2016'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePropertyFillFormatDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // FillFormat özelliğini göstermek için bir dikdörtgen şekli ekleyin
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 100);

            try
            {
                // FillFormat özelliğine erişin (yalnızca okuma)
                MsoFillFormat fillFormat = shape.FillFormat;

                // Mevcut FillFormat özelliklerini görüntüleyin
                Console.WriteLine("FillFormat ForeColor: " + fillFormat.ForeColor);
                Console.WriteLine("FillFormat Transparency: " + fillFormat.Transparency);
                Console.WriteLine("FillFormat BackColor: " + fillFormat.BackColor);
                Console.WriteLine("FillFormat IsVisible: " + fillFormat.IsVisible);

                // FillFormat özelliklerini değiştirin (çünkü yalnızca okuma değildir)
                fillFormat.ForeColor = System.Drawing.Color.Red;
                fillFormat.Transparency = 0.5;
                fillFormat.BackColor = System.Drawing.Color.Yellow;
                fillFormat.IsVisible = true;

                // Güncellenmiş FillFormat özelliklerini görüntüleyin
                Console.WriteLine("Updated FillFormat ForeColor: " + fillFormat.ForeColor);
                Console.WriteLine("Updated FillFormat Transparency: " + fillFormat.Transparency);
                Console.WriteLine("Updated FillFormat BackColor: " + fillFormat.BackColor);
                Console.WriteLine("Updated FillFormat IsVisible: " + fillFormat.IsVisible);

                // Çalışma kitabını kaydedin
                workbook.Save("FillFormatDemo.xlsx");
                Console.WriteLine("FillFormat has been demonstrated and workbook saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [MsoFillFormat](../../msofillformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


