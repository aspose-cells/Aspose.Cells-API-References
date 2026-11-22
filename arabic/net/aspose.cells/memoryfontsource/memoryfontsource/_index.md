---
title: "MemoryFontSource.MemoryFontSource"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ MemoryFontSource. Ctor"
type: docs
url: /ar/net/aspose.cells/memoryfontsource/memoryfontsource/
---
## MemoryFontSource constructor

منشئ.

```csharp
public MemoryFontSource(byte[] fontData)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fontData | Byte[] | بيانات الخط الثنائية. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class MemoryFontSourceMethodCtorWithByteArrayDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            try
            {
                // تحميل ملف خط TrueType إلى مصفوفة بايت
                byte[] fontData = File.ReadAllBytes("arial.ttf");
                
                // استدعاء طريقة #ctor مع معامل مصفوفة بايت
                MemoryFontSource fontSource = new MemoryFontSource(fontData);
                
                // تعيين مصادر الخط باستخدام الفئة الثابتة FontConfigs
                FontConfigs.SetFontSources(new FontSourceBase[] { fontSource });
                
                // تحقق من خصائص مصدر الخط
                Console.WriteLine($"Font source type: {fontSource.Type}");
                Console.WriteLine($"Font data length: {fontSource.FontData.Length} bytes");
                
                // استخدام الخط في خلية
                Worksheet worksheet = workbook.Worksheets[0];
                var style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 14;
                worksheet.Cells["A1"].PutValue("Text with custom font");
                worksheet.Cells["A1"].SetStyle(style);
                
                Console.WriteLine("MemoryFontSource constructor executed successfully with byte array parameter");
            }
            catch (FileNotFoundException ex)
            {
                Console.WriteLine($"Error: Font file not found. {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing MemoryFontSource constructor: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("MemoryFontSourceCtorDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [MemoryFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


