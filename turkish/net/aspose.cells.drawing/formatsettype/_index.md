---
title: "Enum FormatSetType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.FormatSetType enum. Doldurma biçimi kümesi türü"
type: docs
url: /tr/net/aspose.cells.drawing/formatsettype/
---
## FormatSetType enumeration

Dolgu biçim küme türü.

```csharp
public enum FormatSetType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | Doldurma yok biçimi. |
| IsGradientSet | `1` | Gradyan doldurma biçimi. |
| IsTextureSet | `2` | Doku doldurma biçimi. |
| IsPatternSet | `3` | Desen doldurma biçimi. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassFormatSetTypeDemo
    {
        public static void Run()
        {
            // Demonstrasyon için yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Doldurma biçimini göstermek için bir şekil ekle
                Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 200, 200);
                FillFormat fillFormat = shape.Fill;

                // İlk doldurma türünü göster
                Console.WriteLine("Initial fill type: " + fillFormat.Type);

                // FormatSetType enum değerlerini göster
                Console.WriteLine("FormatSetType.None: " + (int)FormatSetType.None);
                Console.WriteLine("FormatSetType.IsGradientSet: " + (int)FormatSetType.IsGradientSet);
                Console.WriteLine("FormatSetType.IsTextureSet: " + (int)FormatSetType.IsTextureSet);
                Console.WriteLine("FormatSetType.IsPatternSet: " + (int)FormatSetType.IsPatternSet);

                // FormatSetType kullanarak farklı doldurma türlerini uygula
                fillFormat.Type = (FillType)FormatSetType.IsGradientSet;
                Console.WriteLine("After setting gradient: " + fillFormat.Type);

                fillFormat.Type = (FillType)FormatSetType.IsPatternSet;
                Console.WriteLine("After setting pattern: " + fillFormat.Type);

                // Çalışma kitabını kaydedin
                workbook.Save("FormatSetTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with FormatSetType: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


