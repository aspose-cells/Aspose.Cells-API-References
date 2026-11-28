---
title: "PictureBulletValue.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PictureBulletValue özelliği. Mermi değerinin tipini alır"
type: docs
url: /tr/net/aspose.cells.drawing.texts/picturebulletvalue/type/
---
## PictureBulletValue.Type property

Madde işaretinin değerinin tipini alır.

```csharp
public override BulletType Type { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class PictureBulletValuePropertyTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // PictureBulletValue örneği oluştur
                PictureBulletValue bulletValue = new PictureBulletValue();
                
                // Type özelliği değerini göster (yalnızca okuma işlemi)
                Console.WriteLine("PictureBulletValue Type: " + bulletValue.Type);
                
                // Bu sınıf için Type'ın Picture olarak doğru şekilde ayarlandığını göster
                if (bulletValue.Type == BulletType.Picture)
                {
                    Console.WriteLine("Type is correctly set to Picture for PictureBulletValue");
                }
                
                // Çalışma kitabını kaydedin
                workbook.Save("PictureBulletValueTypeDemo.xlsx");
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

* enum [BulletType](../../bullettype/)
* class [PictureBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


