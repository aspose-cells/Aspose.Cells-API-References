---
title: "الفئة ExternalLink"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.ExternalLink. تمثل ارتباطًا خارجيًا في مصنف"
type: docs
url: /ar/net/aspose.cells/externallink/
---
## ExternalLink class

يمثل رابطًا خارجيًا في المصنف.

```csharp
public class ExternalLink
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [DataSource](../../aspose.cells/externallink/datasource/) { get; set; } | يمثل مصدر البيانات للارتباط الخارجي. |
| [IsReferred](../../aspose.cells/externallink/isreferred/) { get; } | يشير إلى ما إذا كان هذا الارتباط الخارجي مُشارًا إليه من قبل آخرين. |
| [IsVisible](../../aspose.cells/externallink/isvisible/) { get; } | يشير إلى ما إذا كان هذا الارتباط الخارجي مرئيًا في MS Excel. |
| [OriginalDataSource](../../aspose.cells/externallink/originaldatasource/) { get; set; } | يمثل مصدر البيانات المخزن للارتباط الخارجي. |
| [PathType](../../aspose.cells/externallink/pathtype/) { get; } | احصل على نوع المسار لهذا الارتباط الخارجي |
| [Type](../../aspose.cells/externallink/type/) { get; } | يحصل على نوع الارتباط الخارجي. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [AddExternalName](../../aspose.cells/externallink/addexternalname/)(string, string) | يضيف اسمًا خارجيًا. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExternalLinkDemo
    {
        public static void ExternalLinkExample()
        {
            // فتح ملف يحتوي على روابط خارجية
            Workbook workbook = new Workbook("UpdatedExternalLinkExample_original.xlsx");

            // الحصول على الرابط الخارجي 
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];

            // عرض خصائص الارتباط الخارجي
            Console.WriteLine("External Link Type: " + externalLink.Type);
            Console.WriteLine("Path Type: " + externalLink.PathType);
            Console.WriteLine("Original Data Source: " + externalLink.OriginalDataSource);
            Console.WriteLine("Data Source: " + externalLink.DataSource);
            Console.WriteLine("Is Referred: " + externalLink.IsReferred);
            Console.WriteLine("Is Visible: " + externalLink.IsVisible);

            // تغيير مصدر بيانات الرابط الخارجي
            externalLink.DataSource = "d:\\linktest.xls";

            // إضافة اسم خارجي إلى الارتباط الخارجي
            externalLink.AddExternalName("ExternalName", "Sheet1!A1");

            // احفظ المصنف
            workbook.Save("UpdatedExternalLinkExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


