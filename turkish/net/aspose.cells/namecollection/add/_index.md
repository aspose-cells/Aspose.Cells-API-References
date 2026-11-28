---
title: "NameCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "NameCollection yöntemi. Yeni bir ad tanımlar"
type: docs
url: /tr/net/aspose.cells/namecollection/add/
---
## NameCollection.Add method

Yeni bir ad tanımlar.

```csharp
public int Add(string text)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| metin | String | Ad olarak kullanılacak metin. |

### Dönüş Değeri

[`Name`](../../name/) object index.

### Açıklamalar

Ad boşluk içeremez ve hücre referansı gibi görünemez.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook(FileFormatType.Xlsx);
            Worksheet worksheet = wb.Worksheets[0];
            
            // Dize referansı ile bir ad ekleyin
            int index = wb.Worksheets.Names.Add("MyNamedRange");
            Name namedRange = wb.Worksheets.Names[index];
            
            // Adın başvurduğu formülü ayarlayın
            namedRange.RefersTo = "=Sheet1!$A$1:$B$10";
            
            // Sonuçları doğrulayın ve çıktı verin
            Console.WriteLine("Named Range RefersTo: " + namedRange.RefersTo);
            Console.WriteLine("Named Range Index: " + index);
            
            // Aralığı alın ve adresini gösterin
            Aspose.Cells.Range range = namedRange.GetRange();
            Console.WriteLine("Range Address: " + range.Address);
        }
    }
}
```

### Ayrıca Bakınız

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


