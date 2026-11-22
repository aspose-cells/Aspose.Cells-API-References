---
title: "XmlSaveOptions.XmlMapName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية XmlSaveOptions. تشير إلى ما إذا كان يتم تصرف خريطة xml في الملف"
type: docs
url: /ar/net/aspose.cells/xmlsaveoptions/xmlmapname/
---
## XmlSaveOptions.XmlMapName property

يشير إلى ما إذا كان يتم تصدير خريطة XML في الملف.

```csharp
public string XmlMapName { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlSaveOptionsPropertyXmlMapNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ملء بعض البيانات في ورقة العمل
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);

            // إنشاء خريطة XML وإضافتها إلى المصنف
            int mapIndex = workbook.Worksheets.XmlMaps.Add("<Schema><Element><Product/><Price/></Element></Schema>");
            XmlMap xmlMap = workbook.Worksheets.XmlMaps[mapIndex];
            xmlMap.Name = "ProductDataMap";

            // إنشاء XmlSaveOptions وتعيين XmlMapName
            XmlSaveOptions saveOptions = new XmlSaveOptions();
            saveOptions.XmlMapName = "ProductDataMap";

            // حفظ المصنف باستخدام تخطيط XML
            workbook.Save("XmlWithMapping.xml", saveOptions);
        }
    }
}
```

### انظر أيضًا

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


