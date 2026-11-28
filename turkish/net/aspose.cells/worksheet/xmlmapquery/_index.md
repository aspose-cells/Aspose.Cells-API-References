---
title: "Worksheet.XmlMapQuery"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet yöntemi. XML haritasının belirli yoluna eşlenen/bağlanan hücre alanlarını sorgulayın"
type: docs
url: /tr/net/aspose.cells/worksheet/xmlmapquery/
---
## Worksheet.XmlMapQuery method

Belirli bir XML harita yoluna eşlenen/bağlanan hücre alanlarını sorgular.

```csharp
[Obsolete("Use Worksheet.GetAreasOfXmlMapQuery() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList XmlMapQuery(string path, XmlMap xmlMap)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yol | String | xml öğe yolu |
| xmlMap | XmlMap | Belirli bir harita içinde belirli bir yol için sorgulama yapmak istiyorsanız bir xml haritası belirtin |

### Dönüş Değeri

[`CellArea`](../../cellarea/) list that mapped/linked to the specific path of xml map, an empty list is returned if nothing is mapped/linked.

### Açıklamalar

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Worksheet.GetAreasOfXmlMapQuery() yöntemini kullanın. Bu özellik, Ağustos 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodXmlMapQueryWithStringXmlMapDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek bir XML haritası oluşturun
            string xml = @"<?xml version='1.0' encoding='UTF-8'?>
                <ns1:Root xmlns:ns1='http://example.com'>
                    <ns1:Data>
                        <ns1:Item>Value1</ns1:Item>
                    </ns1:Data>
                </ns1:Root>";
            
            // Haritayı oluşturmak için XML içe aktarın
            workbook.ImportXml(xml, "Sheet1", 0, 0);
            
            // XML haritasını alın
            XmlMap xmlMap = workbook.Worksheets.XmlMaps[0];
            
            // XML haritasını sorgulayın
            ArrayList cellAreas = worksheet.XmlMapQuery("/ns1:Root/ns1:Data/ns1:Item", xmlMap);
            
            // Sonuçları çıktı olarak ver
            if (cellAreas.Count > 0)
            {
                CellArea area = (CellArea)cellAreas[0];
                Console.WriteLine($"Found data at row {area.StartRow}, column {area.StartColumn}");
                Console.WriteLine($"Cell value: {worksheet.Cells[area.StartRow, area.StartColumn].StringValue}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [XmlMap](../../xmlmap/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


