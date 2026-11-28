---
title: "StyleFlag.Alignments"
second_title: "Aspose.Cells için .NET API Referansı"
description: "StyleFlag özelliği. Hizalama ayarı uygulanacak"
type: docs
url: /tr/net/aspose.cells/styleflag/alignments/
---
## StyleFlag.Alignments property

Hizalama ayarı uygulanacak.

```csharp
public bool Alignments { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyAlignmentsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresine erişin ve bazı metinler ayarlayın
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // Bir stil nesnesi oluşturun ve hizalama özelliklerini ayarlayın
            Style style = workbook.CreateStyle();
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.RotationAngle = 45;

            // Bir stil bayrağı oluşturun ve hizalama özelliklerini etkinleştirin
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Alignments = true;

            // Stil bayrağıyla stili hücreye uygulayın
            cell.SetStyle(style, styleFlag);

            // Mevcut hizalama ayarlarını göster
            Console.WriteLine("Horizontal Alignment: " + cell.GetStyle().HorizontalAlignment);
            Console.WriteLine("Vertical Alignment: " + cell.GetStyle().VerticalAlignment);
            Console.WriteLine("Rotation: " + cell.GetStyle().RotationAngle);

            // Stil bayrağını değiştirerek hizalama özelliklerini devre dışı bırakın
            styleFlag.Alignments = false;
            
            // Farklı hizalama ile yeni bir stil oluşturun
            Style newStyle = workbook.CreateStyle();
            newStyle.HorizontalAlignment = TextAlignmentType.Right;
            newStyle.VerticalAlignment = TextAlignmentType.Top;
            newStyle.RotationAngle = 0;

            // Yeni stili uygulayın - hizalamalar değişmeyecek çünkü bayrak false
            cell.SetStyle(newStyle, styleFlag);

            // Değişmemiş hizalama ayarlarını göster
            Console.WriteLine("After applying new style with Alignments=false:");
            Console.WriteLine("Horizontal Alignment: " + cell.GetStyle().HorizontalAlignment);
            Console.WriteLine("Vertical Alignment: " + cell.GetStyle().VerticalAlignment);
            Console.WriteLine("Rotation: " + cell.GetStyle().RotationAngle);

            // Çalışma kitabını kaydedin
            workbook.Save("StyleFlagAlignmentsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


