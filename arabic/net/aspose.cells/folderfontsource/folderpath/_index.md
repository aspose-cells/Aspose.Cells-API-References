---
title: "FolderFontSource.FolderPath"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FolderFontSource. مسار مجلد الخطوط"
type: docs
url: /ar/net/aspose.cells/folderfontsource/folderpath/
---
## FolderFontSource.FolderPath property

مسار إلى مجلد الخطوط.

```csharp
public string FolderPath { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FolderFontSourcePropertyFolderPathDemo
    {
        public static void Run()
        {
            // إنشاء مصدر خط من مجلد
            string folderPath = @"C:\Windows\Fonts"; // Typical system fonts folder
            bool scanSubfolders = true;
            FolderFontSource folderFontSource = new FolderFontSource(folderPath, scanSubfolders);

            // إظهار استخدام خاصية FolderPath
            Console.WriteLine("Font folder path: " + folderFontSource.FolderPath);
            Console.WriteLine("Scan subfolders: " + folderFontSource.ScanSubFolders);

            // إنشاء مصنف مع مصدر الخط
            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource });

            // عرض بسيط - إضافة نص قد يستخدم خطوطًا مخصصة
            workbook.Worksheets[0].Cells["A1"].PutValue("Font Source Demo");
            
            // احفظ المخرجات
            workbook.Save("FolderFontSourceDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FolderFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


