---
title: "الفئة XmlDataBinding"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.XmlDataBinding. تمثل معلومات ربط بيانات XML"
type: docs
url: /ar/net/aspose.cells/xmldatabinding/
---
## XmlDataBinding class

يمثل معلومات ربط بيانات Xml.

```csharp
public class XmlDataBinding
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Url](../../aspose.cells/xmldatabinding/url/) { get; } | يحصل على عنوان url المصدر لهذا الربط البيانات. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class CellsClassXmlDataBindingDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء كائن قائمة سيستخدم ربط بيانات XML
            ListObject listObject = worksheet.ListObjects[worksheet.ListObjects.Add(0, 0, 5, 4, true)];

            // احصل على معلومات ربط بيانات XML (عادةً ما يتم ضبطها عند استيراد بيانات XML)
            XmlDataBinding xmlDataBinding = listObject.XmlMap.DataBinding;

            // عرض عنوان URL لمصدر بيانات XML (خاصية للقراءة فقط)
            Console.WriteLine("XML Data Binding Source URL: " + xmlDataBinding.Url);

            // ملاحظة: في سيناريو حقيقي، سيتم تعيين عنوان URL عند استيراد بيانات XML
            // لأغراض العرض، نوضح كيفية الوصول إلى الخاصية

            // احفظ المصنف
            workbook.Save("XmlDataBindingDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


