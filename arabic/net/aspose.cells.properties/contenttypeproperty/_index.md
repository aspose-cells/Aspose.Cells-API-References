---
title: "الفئة ContentTypeProperty"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Properties.ContentTypeProperty. تمثل معلومات المعرف"
type: docs
url: /ar/net/aspose.cells.properties/contenttypeproperty/
---
## ContentTypeProperty class

يمثل معلومات المعرف.

```csharp
public class ContentTypeProperty
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [IsNillable](../../aspose.cells.properties/contenttypeproperty/isnillable/) { get; set; } | يشير إلى ما إذا كانت القيمة يمكن أن تكون فارغة. |
| [Name](../../aspose.cells.properties/contenttypeproperty/name/) { get; set; } | إرجاع أو تعيين اسم الكائن. |
| [Type](../../aspose.cells.properties/contenttypeproperty/type/) { get; set; } | الحصول على نوع الخاصية وتعيينه. |
| [Value](../../aspose.cells.properties/contenttypeproperty/value/) { get; set; } | إرجاع أو تعيين قيمة خاصية نوع المحتوى. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class ContentTypePropertyDemo
    {
        public static void ContentTypePropertyExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();

            // إضافة خاصية نوع محتوى جديدة
            workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");

            // الوصول إلى الخاصية التي تم إضافتها حديثًا
            ContentTypeProperty property = workbook.ContentTypeProperties["Admin"];
            
            // ضبط الخصائص
            property.Name = "Admin";
            property.Value = "Aspose";
            property.Type = "text";
            property.IsNillable = true;

            // احفظ ملف Excel
            workbook.Save("ContentTypePropertyExample.xlsx");
            workbook.Save("ContentTypePropertyExample.pdf");
            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


