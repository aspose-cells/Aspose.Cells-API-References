---
title: "تعداد DirectoryType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.DirectoryType. يمثل نوع الدليل لاسم الملف"
type: docs
url: /ar/net/aspose.cells/directorytype/
---
## DirectoryType enumeration

يمثل نوع الدليل لاسم الملف.

```csharp
public enum DirectoryType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Volume | `0` | يمثل حرف محرك أقراص MS-DOS. يتبعه حرف المحرك. أو أسماء ملفات UNC، مثل \\server\share\myfile.xls |
| SameVolume | `1` | يشير إلى أن دفتر العمل المصدر على نفس محرك الأقراص مثل دفتر العمل التابع (يتم حذف حرف المحرك) |
| DownDirectory | `2` | يشير إلى أن دفتر العمل المصدر في دليل فرعي من الدليل الحالي. |
| UpDirectory | `3` | يشير إلى أن دفتر العمل المصدر في الدليل الأب للدليل الحالي. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DirectoryTypeDemo
    {
        public static void DirectoryTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(200);
            worksheet.Cells["A4"].PutValue(300);

            // إضافة رابط خارجي إلى دفتر العمل
            string externalFileName = "externalWorkbook.xlsx";
            string[] sheetNames = { "Sheet1" };

            // إضافة رابط خارجي باستخدام DirectoryType.Volume
            int linkIndex = workbook.Worksheets.ExternalLinks.Add(DirectoryType.Volume, externalFileName, sheetNames);

            // استرجاع الرابط الخارجي المضاف
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[linkIndex];

            // إخراج تفاصيل الرابط الخارجي
            Console.WriteLine("External Link Details:");
            Console.WriteLine("File Name: " + externalLink.DataSource);

            // احفظ المصنف
            workbook.Save("DirectoryTypeExample.xlsx");
            workbook.Save("DirectoryTypeExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


