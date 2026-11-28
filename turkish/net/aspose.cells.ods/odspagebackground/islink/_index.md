---
title: "OdsPageBackground.IsLink"
second_title: "Aspose.Cells için .NET API Referansı"
description: "OdsPageBackground özelliği. Bağlantılı bir grafik olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.ods/odspagebackground/islink/
---
## OdsPageBackground.IsLink property

Bağlantılı bir grafik olup olmadığını gösterir.

```csharp
public bool IsLink { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;

    public class OdsPageBackgroundPropertyIsLinkDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook(FileFormatType.Ods);
            Worksheet worksheet = workbook.Worksheets[0];

            // OdsPageBackground'a erişin
            OdsPageBackground background = worksheet.PageSetup.ODSPageBackground;

            // Mevcut IsLink değerini gösterin
            Console.WriteLine("Current IsLink value: " + background.IsLink);

            // Yeni bir tane oluşturmak yerine mevcut arka plan özelliklerini değiştirin
            background.Type = OdsPageBackgroundType.Graphic;
            background.GraphicType = OdsPageBackgroundGraphicType.Position;
            background.GraphicPositionType = OdsPageBackgroundGraphicPositionType.TopLeft;
            background.LinkedGraphic = "path/to/image.png";

            // Yeni IsLink değerini gösterin
            Console.WriteLine("New IsLink value: " + worksheet.PageSetup.ODSPageBackground.IsLink);

            // Sonucu kaydet
            workbook.Save("OdsPageBackgroundIsLinkDemo.ods");
        }
    }
}
```

### Ayrıca Bakınız

* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


