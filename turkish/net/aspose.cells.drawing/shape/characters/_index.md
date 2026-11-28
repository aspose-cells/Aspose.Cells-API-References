---
title: "Shape.Characters"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape yöntemi. Metin içinde bir karakter aralığını temsil eden bir Characters nesnesi döndürür"
type: docs
url: /tr/net/aspose.cells.drawing/shape/characters/
---
## Shape.Characters method

Metin içindeki bir karakter aralığını temsil eden Characters nesnesini döndürür

```csharp
public FontSetting Characters(int startIndex, int length)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startIndex | Int32 | Karakterin başlangıç indeksidir. |
| uzunluk | Int32 | Karakter sayısı. |

### Dönüş Değeri

Karakterler nesnesi.

### Açıklamalar

Bu yöntem yalnızca başlıklı şekil üzerinde çalışır.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodCharactersWithInt32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Metin içeren bir şekil ekleyin
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);
            shape.Text = "Sample Text";

            // 0. indeksten 4 uzunluğunda karakterleri al
            FontSetting fontSetting = shape.Characters(0, 4);
            
            // Yazı tipi ayarlarını değiştir
            fontSetting.Font.Color = System.Drawing.Color.Red;
            fontSetting.Font.Size = 14;
            fontSetting.Font.IsBold = true;

            // Çalışma kitabını kaydedin
            workbook.Save("ShapeCharactersDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


