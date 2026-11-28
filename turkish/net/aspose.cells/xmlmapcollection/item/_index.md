---
title: "XmlMapCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "XmlMapCollection özelliği. Belirli bir dizine göre xml haritasını alır"
type: docs
url: /tr/net/aspose.cells/xmlmapcollection/item/
---
## XmlMapCollection indexer

Belirli indeks ile xml haritasını alır.

```csharp
public XmlMap this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | İndeks. |

### Dönüş Değeri

Xml haritası

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlMapCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabından XmlMapCollection'a erişin
            XmlMapCollection xmlMaps = workbook.Worksheets.XmlMaps;

            // Koleksiyona yeni bir XmlMap ekleyin
            int xmlMapIndex = xmlMaps.Add("data.xsd");

            // Item özelliğini kullanarak XmlMap'e erişin
            XmlMap xmlMap = xmlMaps[xmlMapIndex];

            // XmlMap'in adını göster
            Console.WriteLine("XmlMap Name: " + xmlMap.Name);

            // Çalışma kitabını kaydedin
            workbook.Save("XmlMapCollectionExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [XmlMap](../../xmlmap/)
* class [XmlMapCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


