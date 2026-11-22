---
title: "Workbook.ImportXml"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. تستورد/تحدّث ملف بيانات XML إلى المصنف"
type: docs
url: /ar/net/aspose.cells/workbook/importxml/
---
## ImportXml(string, string, int, int) {#importxml_1}

يستورد/يحدّث ملف بيانات XML إلى المصنف.

```csharp
public void ImportXml(string url, string sheetName, int row, int col)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| url | String | عنوان URL/المسار لملف XML. |
| sheetName | String | اسم الورقة الوجهة. |
| صف | Int32 | الصف الوجهة |
| عمود | Int32 | العمود الوجهة |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodImportXmlWithStringStringInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء كائن دفتر عمل
            Workbook wb = new Workbook();
            
            // استيراد بيانات XML إلى الورقة الأولى بدءًا من الخلية A1
            wb.ImportXml("data.xml", "Sheet1", 0, 0);
            
            // احفظ المصنف
            wb.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportXml(Stream, string, int, int) {#importxml}

يستورد/يحدّث ملف بيانات XML إلى المصنف.

```csharp
public void ImportXml(Stream stream, string sheetName, int row, int col)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| تدفق | Stream | دفق ملف XML. |
| sheetName | String | اسم الورقة الوجهة. |
| صف | Int32 | الصف الوجهة. |
| عمود | Int32 | العمود الوجهة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class WorkbookMethodImportXmlWithStreamStringInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إنشاء بيانات XML نموذجية
            string xmlData = @"<Products>
                <Product>
                    <Name>Laptop</Name>
                    <Price>999.99</Price>
                </Product>
                <Product>
                    <Name>Phone</Name>
                    <Price>699.99</Price>
                </Product>
            </Products>";

            // تحويل سلسلة XML إلى MemoryStream
            MemoryStream xmlStream = new MemoryStream();
            StreamWriter writer = new StreamWriter(xmlStream);
            writer.Write(xmlData);
            writer.Flush();
            xmlStream.Position = 0;

            try
            {
                // استيراد بيانات XML إلى المصنف بدءًا من الخلية A1 في الورقة الأولى
                workbook.ImportXml(xmlStream, "Sheet1", 0, 0);

                // احفظ المصنف
                workbook.Save("ImportXmlDemo.xlsx");
                Console.WriteLine("XML data imported successfully to ImportXmlDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing XML: {ex.Message}");
            }
            finally
            {
                // تنظيف الموارد
                xmlStream.Dispose();
            }
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


