---
title: "Worksheet.XmlMapQuery"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Worksheet. استعلام عن مناطق الخلايا التي تم ربطها/توصيلها بالمسار المحدد لخريطة xml"
type: docs
url: /ar/net/aspose.cells/worksheet/xmlmapquery/
---
## Worksheet.XmlMapQuery method

يستعلم عن مناطق الخلايا التي تم ربطها/تخطيطها إلى المسار المحدد لخريطة XML.

```csharp
[Obsolete("Use Worksheet.GetAreasOfXmlMapQuery() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList XmlMapQuery(string path, XmlMap xmlMap)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المسار | String | مسار عنصر xml |
| xmlMap | XmlMap | حدد خريطة xml إذا كنت تريد الاستعلام عن المسار المحدد داخل خريطة معينة |

### قيمة الإرجاع

[`CellArea`](../../cellarea/) list that mapped/linked to the specific path of xml map, an empty list is returned if nothing is mapped/linked.

### ملاحظات

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة Worksheet.GetAreasOfXmlMapQuery(). سيتم إزالة هذه الخاصية بعد 12 شهرًا اعتبارًا من أغسطس 2026. تُعرب Aspose عن أسفها لأي إزعاج قد تكون قد واجهته.

### أمثلة

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
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // أضف ورقة عمل
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء خريطة XML نموذجية
            string xml = @"<?xml version='1.0' encoding='UTF-8'?>
                <ns1:Root xmlns:ns1='http://example.com'>
                    <ns1:Data>
                        <ns1:Item>Value1</ns1:Item>
                    </ns1:Data>
                </ns1:Root>";
            
            // استيراد XML لإنشاء الخريطة
            workbook.ImportXml(xml, "Sheet1", 0, 0);
            
            // الحصول على خريطة XML
            XmlMap xmlMap = workbook.Worksheets.XmlMaps[0];
            
            // استعلام خريطة XML
            ArrayList cellAreas = worksheet.XmlMapQuery("/ns1:Root/ns1:Data/ns1:Item", xmlMap);
            
            // إخراج النتائج
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

### انظر أيضًا

* class [XmlMap](../../xmlmap/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


