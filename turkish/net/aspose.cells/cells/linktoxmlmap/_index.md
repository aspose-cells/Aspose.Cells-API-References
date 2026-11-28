---
title: "Cells.LinkToXmlMap"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Bir XML haritasına bağlan"
type: docs
url: /tr/net/aspose.cells/cells/linktoxmlmap/
---
## Cells.LinkToXmlMap method

Bir XML haritasına bağlantı.

```csharp
public void LinkToXmlMap(string mapName, int row, int column, string path)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| mapName | String | XML haritasının adı |
| satır | Int32 | Hedef hücrenin satırı |
| sütun | Int32 | hedef hücrenin sütunu |
| yol | String | xml haritasındaki xml öğesinin yolu |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodLinkToXmlMapWithStringInt32Int32StringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            
            // Örnek bir XML haritası ekle
            int mapIndex = wb.Worksheets.XmlMaps.Add("<Transmittals><Issued_Document>Test</Issued_Document></Transmittals>");
            XmlMap xmlMap = wb.Worksheets.XmlMaps[mapIndex];
            xmlMap.Name = "Transmittals_Map";
            
            // İlk çalışma sayfasını al
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Hücreyi XML haritasına bağla
            cells.LinkToXmlMap("Transmittals_Map", 0, 0, "/Transmittals/Issued_Document");
            
            // Çalışma kitabını kaydedin
            wb.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


