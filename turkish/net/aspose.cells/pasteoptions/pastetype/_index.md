---
title: "PasteOptions.PasteType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PasteOptions özelliği. Özel yapıştırma türü"
type: docs
url: /tr/net/aspose.cells/pasteoptions/pastetype/
---
## PasteOptions.PasteType property

Yapıştırma özel türü.

```csharp
public PasteType PasteType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertyPasteTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Kaynak değeri ayarla
            worksheet.Cells["A1"].PutValue("SourceValue");

            // Tam nitelikli tip adlarıyla aralıklar oluştur
            Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1");
            Aspose.Cells.Range targetRange = worksheet.Cells.CreateRange("B1:D3");

            // PasteType.All ile kopyala
            targetRange.Copy(sourceRange, new PasteOptions() { PasteType = PasteType.All });

            // Sonuçları çıktı olarak ver
            Console.WriteLine("A1: " + worksheet.Cells["A1"].StringValue);
            Console.WriteLine("B1: " + worksheet.Cells["B1"].StringValue);
            Console.WriteLine("C2: " + worksheet.Cells["C2"].StringValue);
            Console.WriteLine("D3: " + worksheet.Cells["D3"].StringValue);
        }
    }
}
```

### Ayrıca Bakınız

* enum [PasteType](../../pastetype/)
* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


