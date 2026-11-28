---
title: "FillFormat.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FillFormat özelliği. Doldurma tipini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/fillformat/type/
---
## FillFormat.Type property

Doldurma tipini alır ve ayarlar.

```csharp
[Obsolete("Use FillFormat.FillType  instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public FillType Type { get; set; }
```

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine, lütfen FillFormat.FillType özelliğini kullanın. Bu özellik Temmuz 2016'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class FillFormatPropertyTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir dikdörtgen şekli ekle
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 200);
            FillFormat fill = shape.Fill;

            // Mevcut Type değerini göster
            Console.WriteLine("Current Type value: " + fill.Type);

            // Type'ı Gradient'e değiştir (gösterim için kullanılan kullanımdan kaldırılmış özellik)
            fill.Type = FillType.Gradient;

            // İki renkli degrade etkisini uygula
            fill.SetTwoColorGradient(Color.Blue, Color.Green, GradientStyleType.Horizontal, 1);

            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("FillFormatTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [FillType](../../filltype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


