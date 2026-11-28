---
title: "StyleFlag.Locked"
second_title: "Aspose.Cells için .NET API Referansı"
description: "StyleFlag özelliği. Kilitli ayarı uygulanacak"
type: docs
url: /tr/net/aspose.cells/styleflag/locked/
---
## StyleFlag.Locked property

Kilitli ayar uygulanacak.

```csharp
public bool Locked { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyLockedDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Bir stil oluşturun ve kilitli özelliğini ayarlayın
            Style style = workbook.CreateStyle();
            style.IsLocked = true;

            // Bir stil bayrağı oluşturun ve kilitli bayrağı etkinleştirin
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Locked = true;

            // Stili A1 hücresine uygula
            Cell cell = cells["A1"];
            cell.SetStyle(style, styleFlag);

            // Kilitli durumunu doğrulayın
            Console.WriteLine("Cell A1 is locked: " + cell.GetStyle().IsLocked);

            // Kilitleme etkisini görmek için çalışma sayfasını koruyun
            worksheet.Protect(ProtectionType.All);

            // Kilitli hücreyi değiştirmeyi deneyin (çalışma sayfası korunduğunda istisna fırlatır)
            try
            {
                cell.PutValue("Test");
                Console.WriteLine("Cell modified successfully (worksheet not properly protected)");
            }
            catch
            {
                Console.WriteLine("Could not modify locked cell (worksheet protected)");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


