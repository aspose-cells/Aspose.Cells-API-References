---
title: "Shape.FormatCharacters"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape metodu. Bazı karakterleri yazı tipi ayarıyla biçimlendirir"
type: docs
url: /tr/net/aspose.cells.drawing/shape/formatcharacters/
---
## Shape.FormatCharacters method

Bazı karakterleri yazı tipi ayarıyla biçimlendirir.

```csharp
public void FormatCharacters(int startIndex, int length, Font font, StyleFlag flag)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startIndex | Int32 | Başlangıç indeksi. |
| uzunluk | Int32 | Uzunluk. |
| yazı tipi | Yazı Tipi | Yazı tipi ayarı. |
| bayrak | StyleFlag | Yazı tipi ayarının bayrağı. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodFormatCharactersWithInt32Int32FontStyleFlagDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasına bir metin kutusu ekle
            Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);
            textBox.Text = "Sample Text Formatting";
            
            // İstenen özelliklere sahip bir yazı tipi oluşturun
            Aspose.Cells.Font font = textBox.Font;
            font.Name = "Arial";
            font.Size = 12;
            font.IsBold = true;
            
            // Uygulanacak özellikleri belirtmek için stil bayrağı oluşturun
            StyleFlag flag = new StyleFlag();
            flag.FontName = true;
            flag.FontSize = true;
            flag.FontBold = true;
            
            // Belirli karakterlere biçimlendirme uygulayın
            textBox.FormatCharacters(0, 6, font, flag);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Font](../../../aspose.cells/font/)
* class [StyleFlag](../../../aspose.cells/styleflag/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


