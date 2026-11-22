---
title: "XmlLoadOptions.XmlLoadOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ XmlLoadOptions. يمثل خيارات تحميل ملف xml"
type: docs
url: /ar/net/aspose.cells/xmlloadoptions/xmlloadoptions/
---
## XmlLoadOptions() {#constructor}

يمثل خيارات تحميل ملف XML.

```csharp
public XmlLoadOptions()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // إنشاء خيارات تحميل XML جديدة
            XmlLoadOptions options = new XmlLoadOptions();
            
            // تعيين لتحويل القيم الرقمية أو التاريخية
            options.ConvertNumericOrDate = true;
            
            // تحميل دفتر العمل مع الخيارات
            Workbook workbook = new Workbook("input.xml", options);
            
            // الوصول إلى بيانات الخلية
            Cell cell = workbook.Worksheets[0].Cells["A1"];
            Console.WriteLine("Cell Value: " + cell.Value);
            Console.WriteLine("Cell Type: " + cell.Type);
            
            // احفظ دفتر العمل
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## XmlLoadOptions(LoadFormat) {#constructor_1}

يمثل خيارات تحميل ملف XML.

```csharp
public XmlLoadOptions(LoadFormat type)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | LoadFormat | نوع تنسيق التحميل. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XmlLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء مثيل XmlLoadOptions مع معامل LoadFormat
                LoadFormat loadFormat = LoadFormat.Xml;
                XmlLoadOptions xmlLoadOptions = new XmlLoadOptions(loadFormat);

                // تعيين بعض الخصائص لـ XmlLoadOptions
                xmlLoadOptions.StartCell = "A1";
                xmlLoadOptions.IsXmlMap = true;
                xmlLoadOptions.ConvertNumericOrDate = true;

                // إنشاء دفتر عمل باستخدام خيارات التحميل
                Workbook workbook = new Workbook("sample.xml", xmlLoadOptions);

                // الوصول إلى ورقة العمل الأولى
                Worksheet worksheet = workbook.Worksheets[0];

                // عرض بعض المعلومات
                Console.WriteLine("XML file loaded successfully with LoadFormat.Xml");
                Console.WriteLine($"First cell value: {worksheet.Cells["A1"].Value}");

                // احفظ المصنف
                workbook.Save("XmlLoadOptionsCtorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing XmlLoadOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* enum [LoadFormat](../../loadformat/)
* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


