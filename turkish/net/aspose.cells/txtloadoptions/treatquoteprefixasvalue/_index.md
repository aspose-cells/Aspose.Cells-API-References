---
title: "TxtLoadOptions.TreatQuotePrefixAsValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TxtLoadOptions özelliği. Başlangıçtaki tek tırnak işaretinin bir hücrenin değeri içinde yer alıp almayacağını gösterir. Varsayılan true'dur. False ise, ilgili hücrenin değerinden başlangıçtaki tek tırnak kaldırılır ve hücre için QuotePrefix true olarak ayarlanır."
type: docs
url: /tr/net/aspose.cells/txtloadoptions/treatquoteprefixasvalue/
---
## TxtLoadOptions.TreatQuotePrefixAsValue property

Başlangıçtaki tek tırnak işaretinin bir hücrenin değeri içinde yer alıp almayacağını gösterir. Varsayılan true'dur. False ise, ilgili hücrenin değerinden başlangıçtaki tek tırnak kaldırılır ve [`QuotePrefix`](../../style/quoteprefix/) true olarak hücreye ayarlanır.

```csharp
public bool TreatQuotePrefixAsValue { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyTreatQuotePrefixAsValueDemo
    {
        public static void Run()
        {
            // Alıntı önekleriyle örnek CSV verisi oluştur
            string csvData = "ID,Name,Value\n1,\"'Apple\",100\n2,\"'Orange\",200";
            string filePath = "test.csv";

            // CSV verisini bir dosyaya kaydet
            File.WriteAllText(filePath, csvData);

            // Senaryo 1: TreatQuotePrefixAsValue = false (varsayılan)
            var loadOptions1 = new TxtLoadOptions();
            loadOptions1.TreatQuotePrefixAsValue = false;
            
            var workbook1 = new Workbook(filePath, loadOptions1);
            var worksheet1 = workbook1.Worksheets[0];
            Console.WriteLine("TreatQuotePrefixAsValue = false:");
            Console.WriteLine("Cell B2 value: " + worksheet1.Cells["B2"].Value); // Will show 'Apple (quote treated as formatting)

            // Senaryo 2: TreatQuotePrefixAsValue = true
            var loadOptions2 = new TxtLoadOptions();
            loadOptions2.TreatQuotePrefixAsValue = true;
            
            var workbook2 = new Workbook(filePath, loadOptions2);
            var worksheet2 = workbook2.Worksheets[0];
            Console.WriteLine("\nTreatQuotePrefixAsValue = true:");
            Console.WriteLine("Cell B2 value: " + worksheet2.Cells["B2"].Value); // Will show 'Apple (quote treated as value)

            // Temizle
            File.Delete(filePath);
        }
    }
}
```

### Ayrıca Bakınız

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


