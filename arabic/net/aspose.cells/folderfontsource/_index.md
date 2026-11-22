---
title: "فئة FolderFontSource"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.FolderFontSource. تمثل المجلد الذي يحتوي على ملفات خطوط TrueType"
type: docs
url: /ar/net/aspose.cells/folderfontsource/
---
## FolderFontSource class

يمثل المجلد الذي يحتوي على ملفات خطوط TrueType.

```csharp
public class FolderFontSource : FontSourceBase
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [FolderFontSource](folderfontsource/)(string, bool) | منشئ. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [FolderPath](../../aspose.cells/folderfontsource/folderpath/) { get; } | مسار إلى مجلد الخطوط. |
| [ScanSubFolders](../../aspose.cells/folderfontsource/scansubfolders/) { get; } | يحدد ما إذا كان يجب مسح المجلدات الفرعية أم لا. |
| override [Type](../../aspose.cells/folderfontsource/type/) { get; } | يرجع نوع مصدر الخط. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FolderFontSourceDemo
    {
        public static void FolderFontSourceExample()
        {
            // إنشاء مثال من FolderFontSource
            string folderPath = @"C:\Fonts";
            bool scanSubfolders = true;
            FolderFontSource folderFontSource = new FolderFontSource(folderPath, scanSubfolders);

            // الوصول إلى الخصائص
            Console.WriteLine("Folder Path: " + folderFontSource.FolderPath);
            Console.WriteLine("Scan Subfolders: " + folderFontSource.ScanSubFolders);
            Console.WriteLine("Font Source Type: " + folderFontSource.Type);

            // إنشاء مصنف وتعيين مصادر الخطوط
            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource });

            // احفظ المصنف
            workbook.Save("FolderFontSourceExample.xlsx");
            workbook.Save("FolderFontSourceExample.pdf");
            return;
        }
    }
}
```

### انظر أيضًا

* class [FontSourceBase](../fontsourcebase/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


