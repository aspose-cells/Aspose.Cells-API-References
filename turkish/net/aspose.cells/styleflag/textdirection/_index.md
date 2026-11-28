---
title: "StyleFlag.TextDirection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "StyleFlag özelliği. Metin yönü ayarı uygulanacak"
type: docs
url: /tr/net/aspose.cells/styleflag/textdirection/
---
## StyleFlag.TextDirection property

Metin yönü ayarı uygulanacak.

```csharp
public bool TextDirection { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyTextDirectionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresine erişin ve bazı metinler ayarlayın
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text with TextDirection");

            // Bir stil oluşturun ve metin yönünü ayarlayın
            Style style = workbook.CreateStyle();
            style.TextDirection = TextDirectionType.Context;

            // Bir stil bayrağı oluşturun ve TextDirection bayrağını etkinleştirin
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.TextDirection = true;

            // Stil bayrağıyla stili hücreye uygulayın
            cell.SetStyle(style, styleFlag);

            // Mevcut metin yönünü göster
            Console.WriteLine("Current TextDirection value: " + cell.GetStyle().TextDirection);

            // Metin yönünü değiştirin ve tekrar uygulayın
            style.TextDirection = TextDirectionType.LeftToRight;
            cell.SetStyle(style, styleFlag);

            Console.WriteLine("Current TextDirection value: " + cell.GetStyle().TextDirection);

            // Çalışma kitabını kaydedin
            workbook.Save("TextDirectionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


