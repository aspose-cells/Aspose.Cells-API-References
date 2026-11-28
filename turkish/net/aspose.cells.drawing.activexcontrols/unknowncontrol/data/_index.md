---
title: "UnknownControl.Data"
second_title: "Aspose.Cells için .NET API Referansı"
description: "UnknownControl özelliği. Denetimin ikili verisini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/unknowncontrol/data/
---
## UnknownControl.Data property

Kontrolün ikili verilerini alır ve ayarlar.

```csharp
public override byte[] Data { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class UnknownControlPropertyDataDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Sahte bir CLSID oluştur (geçersiz tanımlayıcı)
            byte[] dummyClsid = new byte[16];

            // ControlType.Unknown kullanarak tam parametrelerle bilinmeyen bir ActiveX denetimi ekle
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.Unknown, 0, 0, 100, 100, 0, 0);

            // UnknownControl örneğine eriş
            UnknownControl unknownControl = (UnknownControl)shape.ActiveXControl;

            // Denetimin verisini, CLSID dahil, mevcut diziye kopyalayarak ayarla
            Array.Copy(dummyClsid, unknownControl.Data, dummyClsid.Length);

            // Data özelliği bilgilerini oku ve göster
            Console.WriteLine($"Unknown control data length: {unknownControl.Data.Length}");
            Console.WriteLine($"Control type: {unknownControl.Type}");

            // Çıktı dosyasında kontrol verilerinin kalıcılığını gösterin
            workbook.Save("UnknownControlDataDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [UnknownControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


