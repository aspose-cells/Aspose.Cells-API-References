---
title: "DocumentPropertyCollection.Contains"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DocumentPropertyCollection yöntemi. Belirtilen ada sahip bir özellik koleksiyonda varsa true döndürür"
type: docs
url: /tr/net/aspose.cells.properties/documentpropertycollection/contains/
---
## DocumentPropertyCollection.Contains method

Koleksiyonda belirtilen adla bir özellik mevcutsa true döndürür.

```csharp
public bool Contains(string name)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | Özelliğin büyük/küçük harfe duyarsız adı. |

### Dönüş Değeri

Özellik koleksiyonda varsa true; aksi takdirde false.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocumentPropertyCollectionMethodContainsWithStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // "RevisionNumber" özelliğinin yerleşik belge özelliklerinde olup olmadığını kontrol et
            bool containsRevision = workbook.BuiltInDocumentProperties.Contains("RevisionNumber");
            Console.WriteLine("Contains 'RevisionNumber': " + containsRevision);
            
            // Bir özel özellik ekle ve varlığını kontrol et
            workbook.CustomDocumentProperties.Add("CustomProperty", "Test Value");
            bool containsCustom = workbook.CustomDocumentProperties.Contains("CustomProperty");
            Console.WriteLine("Contains 'CustomProperty': " + containsCustom);
        }
    }
}
```

### Ayrıca Bakınız

* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


