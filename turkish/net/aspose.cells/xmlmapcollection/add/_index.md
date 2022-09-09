---
title: Add
second_title: Aspose.Cells for .NET API Referansı
description: EkleXmlMapaspose.cells/xmlmap bir xml/xsd dosyasının urlsi/yolu ile.
type: docs
weight: 20
url: /tr/net/aspose.cells/xmlmapcollection/add/
---
## XmlMapCollection.Add method

Ekle[`XmlMap`](../../xmlmap) bir xml/xsd dosyasının url'si/yolu ile.

```csharp
public int Add(string url)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| url | String | bir xml/xsd dosyasının url'si/yolu. |

### Geri dönüş değeri

[`XmlMap`](../../xmlmap) nesne indeksi.

### Örnekler

Aşağıdaki kod iki[`XmlMap`](../../xmlmap) bir xsd dosyası ve bir xml dosyası ile.

```csharp
Workbook wb = new Workbook();

XmlMapCollection xmlMapCollection = wb.Worksheets.XmlMaps;

// Bir xsd dosyası ile bir <see cref="T:Aspose.Cells.XmlMap" /> ekleyin.
xmlMapCollection.Add("schema.xsd");

// Bir xml dosyası ile bir <see cref="T:Aspose.Cells.XmlMap" /> ekleyin.
xmlMapCollection.Add("xml.xml");

wb.Save("twoXmlMaps.xlsx");
```

### Ayrıca bakınız

* class [XmlMapCollection](../../xmlmapcollection)
* ad alanı [Aspose.Cells](../../xmlmapcollection)
* toplantı [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->