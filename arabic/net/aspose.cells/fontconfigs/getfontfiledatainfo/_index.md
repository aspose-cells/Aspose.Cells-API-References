---
title: "FontConfigs.GetFontFileDataInfo"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة FontConfigs. الحصول على معلومات بيانات ملف الخط"
type: docs
url: /ar/net/aspose.cells/fontconfigs/getfontfiledatainfo/
---
## FontConfigs.GetFontFileDataInfo method

احصل على معلومات بيانات ملف الخط.

```csharp
public static FontFileDataInfo GetFontFileDataInfo(string fontName, bool isBold, bool isItalic, 
    bool isExactStyle)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fontName | String | اسم الخط |
| isBold | منطقي | نمط الخط غامق أم لا |
| isItalic | منطقي | نمط الخط مائل أم لا |
| isExactStyle | منطقي | ما إذا كان يجب مطابقة نمط الغامق/المائل المحدد بدقة |

### قيمة الإرجاع

معلومات بيانات ملف الخط.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsMethodGetFontFileDataInfoWithStringBooleanBooleanBooleanDemo
    {
        public static void Run()
        {
            try
            {
                // استدعاء GetFontFileDataInfo مع معلمات محددة (تم تغييرها إلى استدعاء ثابت)
                FontFileDataInfo fontInfo = FontConfigs.GetFontFileDataInfo("Arial", true, false, false);

                // عرض معلومات حول بيانات ملف الخط
                if (fontInfo != null)
                {
                    Console.WriteLine($"Font format type: {fontInfo.FormatType}");
                    Console.WriteLine($"Font data length: {fontInfo.Data?.Length ?? 0} bytes");
                }
                else
                {
                    Console.WriteLine("Font information not available");
                }

                // إظهار التأثير على المصنف
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // تعيين النمط باستخدام الخط الذي فحصناه
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.IsBold = true;
                style.Font.IsItalic = false;
                
                // تطبيق النمط على خلية
                worksheet.Cells["A1"].SetStyle(style);
                worksheet.Cells["A1"].PutValue("Text with Arial Bold");

                // احفظ المصنف
                workbook.Save("FontConfigsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFontFileDataInfo method: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [FontFileDataInfo](../../fontfiledatainfo/)
* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


