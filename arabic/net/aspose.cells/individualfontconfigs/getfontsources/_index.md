---
title: "IndividualFontConfigs.GetFontSources"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة IndividualFontConfigs. تحصل على نسخة من المصفوفة التي تحتوي على قائمة المصادر"
type: docs
url: /ar/net/aspose.cells/individualfontconfigs/getfontsources/
---
## IndividualFontConfigs.GetFontSources method

يحصل على نسخة من المصفوفة التي تحتوي على قائمة المصادر.

```csharp
public FontSourceBase[] GetFontSources()
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IndividualFontConfigsMethodGetFontSourcesDemo
    {
        public static void Run()
        {
            // إنشاء إعدادات خطوط فردية
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // تعيين بعض مصادر الخطوط (مجلدات تحتوي على خطوط)
            string fontFolder1 = @"C:\Windows\Fonts";
            string fontFolder2 = @"D:\CustomFonts";
            fontConfigs.SetFontFolder(fontFolder1, false);
            fontConfigs.SetFontFolder(fontFolder2, true);

            try
            {
                // احصل على مصادر الخط الحالية
                FontSourceBase[] fontSources = fontConfigs.GetFontSources();

                Console.WriteLine("Current font sources:");
                foreach (var source in fontSources)
                {
                    if (source is FolderFontSource folderSource)
                    {
                        Console.WriteLine($"- Folder: {folderSource.FolderPath} (Recursive: {folderSource.ScanSubFolders})");
                    }
                }

                // أنشئ دفتر عمل لتوضيح التأثير
                Workbook workbook = new Workbook(FileFormatType.Xlsx);
                // استخدام إعدادات الخطوط عند إنشاء الأنماط أو العمل مع الخطوط
                // (المصنف لا يحتوي على خاصية FontConfigs، لذا نقوم بإزالة هذا السطر)
                Worksheet worksheet = workbook.Worksheets[0];

                // استخدام خط مخصص قد يكون موجودًا في أحد المجلدات
                Style style = workbook.CreateStyle();
                style.Font.Name = "SomeCustomFont";
                worksheet.Cells["A1"].SetStyle(style);
                worksheet.Cells["A1"].PutValue("Text with custom font");

                Console.WriteLine("Workbook created with custom font configurations.");
                workbook.Save("MethodGetFontSourcesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFontSources method: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [FontSourceBase](../../fontsourcebase/)
* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


