---
title: "PasteOptions.OperationType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PasteOptions özelliği. Aralık yapıştırıldığında işlem türünü alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/pasteoptions/operationtype/
---
## PasteOptions.OperationType property

Aralık yapıştırılırken işlem türünü alır ve ayarlar.

```csharp
public PasteOperationType OperationType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertyOperationTypeDemo
    {
        public static void Run()
        {
            // Örnek veri içeren kaynak çalışma kitabını oluşturun
            Workbook wbOrigin = new Workbook();
            Worksheet sourceSheet = wbOrigin.Worksheets[0];
            sourceSheet.Cells["A1"].PutValue("Source Data");
            sourceSheet.Cells["B2"].PutValue(100);
            
            // Hedef çalışma kitabı oluştur
            Workbook wbDestination = new Workbook();
            Worksheet destSheet = wbDestination.Worksheets[0];
            destSheet.Cells["A1"].PutValue("Destination Data");
            destSheet.Cells["B2"].PutValue(200); // Will be modified by paste operation
            
            // Kopyala/yapıştır için aralıklar oluştur
            var rangeOrigin = sourceSheet.Cells.CreateRange("A1:B3");
            var rangeDestination = destSheet.Cells.CreateRange("A1:B3");
            
            // OperationType gösterimiyle yapıştırma seçenekleri oluştur
            var options = new PasteOptions
            {
                PasteType = PasteType.All,
                OperationType = PasteOperationType.Add // Values will be added (100 + 200 = 300)
            };
            
            // Kopyala/yapıştır işlemini gerçekleştir
            rangeDestination.Copy(rangeOrigin, options);
            
            // Sonucu doğrula
            Console.WriteLine("B2 value after paste with Add operation: " + destSheet.Cells["B2"].IntValue);
            
            // Sonucu kaydet
            wbDestination.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* enum [PasteOperationType](../../pasteoperationtype/)
* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


