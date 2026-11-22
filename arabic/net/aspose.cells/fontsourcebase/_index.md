---
title: "الفئة FontSourceBase"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.FontSourceBase. هذه فئة أساسية مجردة للفئات التي تسمح للمستخدم بتحديد مصادر خطوط مختلفة"
type: docs
url: /ar/net/aspose.cells/fontsourcebase/
---
## FontSourceBase class

هذه فئة أساسية مجردة للفئات التي تسمح للمستخدم بتحديد مصادر خطوط مختلفة

```csharp
public abstract class FontSourceBase
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| abstract [Type](../../aspose.cells/fontsourcebase/type/) { get; } | يرجع نوع مصدر الخط. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFontSourceBaseDemo
    {
        public static void Run()
        {
            // إنشاء مصدر خط من مجلد
            string fontFolder = @"C:\Windows\Fonts";
            FolderFontSource folderSource = new FolderFontSource(fontFolder, true);

            // عرض خصائص مصدر الخط
            Console.WriteLine($"Font folder: {folderSource.FolderPath}");
            Console.WriteLine($"Scan subfolders: {folderSource.ScanSubFolders}");
            Console.WriteLine($"Source type: {folderSource.Type}");

            // إنشاء دفتر عمل وتعيين مصدر الخط
            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderSource });

            // حفظ باستخدام خطوط مخصصة
            workbook.Save("OutputWithCustomFonts.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


