---
title: "Cells.LinkToXmlMap"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. ربط بخريطة xml"
type: docs
url: /ar/net/aspose.cells/cells/linktoxmlmap/
---
## Cells.LinkToXmlMap method

رابط إلى خريطة XML.

```csharp
public void LinkToXmlMap(string mapName, int row, int column, string path)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| mapName | String | اسم خريطة xml |
| صف | Int32 | صف الخلية الوجهة |
| عمود | Int32 | عمود الخلية الوجهة |
| المسار | String | مسار عنصر xml في خريطة xml |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodLinkToXmlMapWithStringInt32Int32StringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook wb = new Workbook();
            
            // إضافة خريطة XML نموذجية
            int mapIndex = wb.Worksheets.XmlMaps.Add("<Transmittals><Issued_Document>Test</Issued_Document></Transmittals>");
            XmlMap xmlMap = wb.Worksheets.XmlMaps[mapIndex];
            xmlMap.Name = "Transmittals_Map";
            
            // احصل على ورقة العمل الأولى
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // ربط الخلية بخريطة XML
            cells.LinkToXmlMap("Transmittals_Map", 0, 0, "/Transmittals/Issued_Document");
            
            // احفظ المصنف
            wb.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


