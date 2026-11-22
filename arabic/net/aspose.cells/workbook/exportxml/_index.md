---
title: "Workbook.ExportXml"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. تصدير بيانات XML المرتبطة بخريطة XML المحددة"
type: docs
url: /ar/net/aspose.cells/workbook/exportxml/
---
## ExportXml(string, string) {#exportxml_1}

تصدير بيانات XML المرتبطة بخريطة XML المحددة.

```csharp
public void ExportXml(string mapName, string path)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| mapName | String | اسم خريطة XML التي تحتاج إلى تصديرها |
| المسار | String | مسار التصدير |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodExportXmlWithStringStringDemo
    {
        public static void Run()
        {
            // إنشاء مصنف وتحميل ملف Excel
            Workbook wb = new Workbook("Book1.xlsx");
            
            // الحصول على أول XmlMap من المصنف
            if (wb.Worksheets.XmlMaps.Count > 0)
            {
                XmlMap xmlMap = wb.Worksheets.XmlMaps[0];
                
                // تصدير بيانات XML باستخدام اسم XmlMap ومسار ملف الإخراج
                wb.ExportXml(xmlMap.Name, "output.xml");
                Console.WriteLine("XML exported successfully to output.xml");
            }
            else
            {
                Console.WriteLine("No XmlMap found in the workbook");
            }
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ExportXml(string, Stream) {#exportxml}

تصدير بيانات XML.

```csharp
public void ExportXml(string mapName, Stream stream)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| mapName | String | اسم خريطة XML التي تحتاج إلى تصديرها |
| تدفق | Stream | دفق التصدير |

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodExportXmlWithStringStreamDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد وإضافة بعض البيانات
            using (Workbook workbook = new Workbook())
            {
                Worksheet sheet = workbook.Worksheets[0];
                sheet.Cells["A1"].PutValue("Id");
                sheet.Cells["B1"].PutValue("Name");
                sheet.Cells["A2"].PutValue(1);
                sheet.Cells["B2"].PutValue("Alice");
                sheet.Cells["A3"].PutValue(2);
                sheet.Cells["B3"].PutValue("Bob");

                // اسم خريطة XML للتصدير – لأغراض العرض نستخدم اسمًا مؤقتًا
                string mapName = "SampleMap";

                try
                {
                    // تصدير خريطة XML إلى ملف باستخدام FileStream (String, Stream overload)
                    string outputPath = "ExportedSample.xml";
                    using (FileStream fs = new FileStream(outputPath, FileMode.Create, FileAccess.Write))
                    {
                        workbook.ExportXml(mapName, fs);
                    }

                    Console.WriteLine($"ExportXml completed successfully. Output saved to '{outputPath}'.");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error during ExportXml: {ex.Message}");
                }
            }
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


