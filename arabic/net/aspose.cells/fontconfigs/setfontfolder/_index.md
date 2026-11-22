---
title: "FontConfigs.SetFontFolder"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة FontConfigs. تحدد مجلد الخطوط"
type: docs
url: /ar/net/aspose.cells/fontconfigs/setfontfolder/
---
## FontConfigs.SetFontFolder method

يعيّن مجلد الخطوط

```csharp
public static void SetFontFolder(string fontFolder, bool recursive)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fontFolder | String | المجلد الذي يحتوي على خطوط TrueType. |
| recursive | منطقي | يحدد ما إذا كان يجب مسح المجلدات الفرعية أم لا. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontConfigsMethodSetFontFolderWithStringBooleanDemo
    {
        public static void Run()
        {
            // تهيئة دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بعض النص إلى الخلية A1
            worksheet.Cells["A1"].PutValue("Sample Text with Custom Font");
            
            // حدد مجلد خطوط مخصص وحدد ما إذا كان يجب تضمين المجلدات الفرعية
            FontConfigs.SetFontFolder("Fonts", true);
            
            // طبق نمط خط قد يستخدم خطوطًا من المجلد المخصص
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "CustomFont"; // Assuming "CustomFont" exists in the Fonts folder
            style.Font.Size = 14;
            worksheet.Cells["A1"].SetStyle(style);
            
            // احفظ المصنف كملف PDF
            workbook.Save("output.pdf", SaveFormat.Pdf);
        }
    }
}
```

### انظر أيضًا

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


