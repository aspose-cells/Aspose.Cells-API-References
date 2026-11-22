---
title: "FontSourceBase.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FontSourceBase. تُرجع نوع مصدر الخط"
type: docs
url: /ar/net/aspose.cells/fontsourcebase/type/
---
## FontSourceBase.Type property

يرجع نوع مصدر الخط.

```csharp
public abstract FontSourceType Type { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontSourceBasePropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء كائن دفتر عمل
            Workbook workbook = new Workbook();
            
            // إنشاء مصدر خط من مجلد
            FolderFontSource folderFontSource = new FolderFontSource("C:\\MyFonts", true);
            
            // اعرض خاصية Type لمصدر الخط
            Console.WriteLine("Font source type: " + folderFontSource.Type);
            
            // إنشاء مصدر خط من ملف
            FileFontSource fileFontSource = new FileFontSource("arial.ttf");
            
            // اعرض خاصية Type لمصدر الخط
            Console.WriteLine("Font source type: " + fileFontSource.Type);
            
            // إنشاء مصدر خط في الذاكرة (مثال باستخدام مصفوفة بايت)
            byte[] fontData = System.IO.File.ReadAllBytes("arial.ttf");
            MemoryFontSource memoryFontSource = new MemoryFontSource(fontData);
            
            // اعرض خاصية Type لمصدر الخط
            Console.WriteLine("Font source type: " + memoryFontSource.Type);
            
            // تعيين مصادر الخط باستخدام الطريقة الساكنة
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource, fileFontSource, memoryFontSource });
            
            // احفظ المصنف
            workbook.Save("FontSourceTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [FontSourceType](../../fontsourcetype/)
* class [FontSourceBase](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


