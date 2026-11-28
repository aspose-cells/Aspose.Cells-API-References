---
title: "XmlMapCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "XmlMapCollection yöntemi. Bir xml/xsd dosyasının url/ yolu ile bir XmlMap ekleyin"
type: docs
url: /tr/net/aspose.cells/xmlmapcollection/add/
---
## XmlMapCollection.Add method

Bir xml/xsd dosyasının url/yolunu kullanarak bir [`XmlMap`](../../xmlmap/) ekleyin.

```csharp
public int Add(string url)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| url | String | xml/xsd dosyasının url/yolu. |

### Dönüş Değeri

[`XmlMap`](../../xmlmap/) object index.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlMapCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            
            XmlMapCollection xmlMapCollection = wb.Worksheets.XmlMaps;
            
            // Şema ve XML dosyalarını kullanarak XML haritaları ekleyin
            xmlMapCollection.Add("schema.xsd");
            xmlMapCollection.Add("xml.xml");
            
            wb.Save("twoXmlMaps.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [XmlMapCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


