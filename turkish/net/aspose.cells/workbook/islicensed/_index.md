---
title: "Workbook.IsLicensed"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook özelliği. Lisansın ayarlanıp ayarlanmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/workbook/islicensed/
---
## Workbook.IsLicensed property

Lisansın ayarlanıp ayarlanmadığını gösterir.

```csharp
public bool IsLicensed { get; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyIsLicensedDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            
            // Çalışma kitabının kullanıldığını göstermek için bazı temel özellikleri ayarla
            wb.Worksheets[0].Name = "Sheet1";
            wb.Worksheets[0].Cells[0, 0].PutValue("Sample Data");
            
            // Çalışma kitabının lisanslı olup olmadığını kontrol et
            Console.WriteLine($"IsLicensed: {wb.IsLicensed}");
            
            // Lisans durumuna göre farklı davranışı göster
            if (wb.IsLicensed)
            {
                Console.WriteLine("Running in licensed mode - full features available");
            }
            else
            {
                Console.WriteLine("Running in evaluation mode - watermarks will appear");
            }

            // İşlevselliği göstermek için bellek akışına kaydet
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Xlsx);
                Console.WriteLine($"Workbook saved successfully (Size: {ms.Length} bytes)");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


