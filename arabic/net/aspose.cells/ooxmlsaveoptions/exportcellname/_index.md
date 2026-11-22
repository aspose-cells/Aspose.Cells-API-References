---
title: "OoxmlSaveOptions.ExportCellName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية OoxmlSaveOptions. تشير إلى ما إذا كان يتم تصدير اسم الخلية إلى ملف Excel2007 .xlsx .xlsm .xltx .xltm. إذا كان من الممكن الوصول إلى ملف الإخراج بواسطة SQL Server DTS يجب أن تكون هذه القيمة true. ضبط القيمة على false سيزيد الأداء بشكل كبير ويقلل حجم الملف عند إنشاء ملفات كبيرة. القيمة الافتراضية هي true"
type: docs
url: /ar/net/aspose.cells/ooxmlsaveoptions/exportcellname/
---
## OoxmlSaveOptions.ExportCellName property

يشير إلى ما إذا كان يتم تصدير اسم الخلية إلى ملف Excel2007 .xlsx (.xlsm, .xltx, .xltm). إذا كان من الممكن الوصول إلى ملف الإخراج بواسطة SQL Server DTS، يجب أن تكون هذه القيمة true. ضبط القيمة إلى false سيزيد الأداء بشكل كبير ويقلل حجم الملف عند إنشاء ملف كبير. القيمة الافتراضية هي true.

```csharp
public bool ExportCellName { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OoxmlSaveOptionsPropertyExportCellNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // ضع بعض البيانات في الخلايا
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B2"].PutValue(123);
            
            // إنشاء خيارات حفظ XLSX مع تمكين ExportCellName
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.ExportCellName = true;
            
            // حفظ المصنف مع تصدير أسماء الخلايا
            workbook.Save("output_with_cellnames.xlsx", saveOptions);
            
            // إنشاء خيارات حفظ أخرى مع تعطيل ExportCellName (الافتراضي)
            OoxmlSaveOptions saveOptions2 = new OoxmlSaveOptions();
            
            // حفظ المصنف دون تصدير أسماء الخلايا
            workbook.Save("output_without_cellnames.xlsx", saveOptions2);
        }
    }
}
```

### انظر أيضًا

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


