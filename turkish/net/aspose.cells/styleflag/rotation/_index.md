---
title: "StyleFlag.Rotation"
second_title: "Aspose.Cells için .NET API Referansı"
description: "StyleFlag özelliği. Döndürme ayarı uygulanacak"
type: docs
url: /tr/net/aspose.cells/styleflag/rotation/
---
## StyleFlag.Rotation property

Döndürme ayarı uygulanacak.

```csharp
public bool Rotation { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyRotationDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresine erişin ve bazı metinler ayarlayın
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Rotated Text");

            // Hücrenin stilini al
            Style style = workbook.CreateStyle();

            // Yeni döndürme değerini ayarla (45 derece)
            style.RotationAngle = 45;

            // Mevcut döndürme değerini göster
            Console.WriteLine("Current Rotation value: " + cell.GetStyle().RotationAngle);            

            // Bir stil bayrağı oluştur ve döndürme bayrağını etkinleştir
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Rotation = true;

            // Stili döndürme ile hücreye uygula
            cell.SetStyle(style, styleFlag);

            Console.WriteLine("after setting style, rotation value: " + cell.GetStyle().RotationAngle);
           
            // Sonucu kaydet
            workbook.Save("PropertyRotationDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


