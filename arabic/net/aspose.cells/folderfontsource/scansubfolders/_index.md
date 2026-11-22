---
title: "FolderFontSource.ScanSubFolders"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FolderFontSource. تحدد ما إذا كان يجب مسح المجلدات الفرعية أم لا"
type: docs
url: /ar/net/aspose.cells/folderfontsource/scansubfolders/
---
## FolderFontSource.ScanSubFolders property

يحدد ما إذا كان يجب مسح المجلدات الفرعية أم لا.

```csharp
public bool ScanSubFolders { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FolderFontSourcePropertyScanSubFoldersDemo
    {
        public static void Run()
        {
            // إنشاء مصدر خطوط من مجلد مع تمكين مسح المجلدات الفرعية
            string folderPath = @"C:\Windows\Fonts"; // Typical system fonts folder
            bool scanSubfolders = true;
            FolderFontSource folderFontSource = new FolderFontSource(folderPath, scanSubfolders);

            // عرض خصائص مصدر الخط
            Console.WriteLine("Folder Path: " + folderFontSource.FolderPath);
            Console.WriteLine("Scan Subfolders: " + folderFontSource.ScanSubFolders);

            // إنشاء مصنف وتعيين مصدر الخطوط
            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource });

            // إظهار الاستخدام عن طريق تعيين بعض النصوص
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Text with fonts from folder source");

            // احفظ المصنف
            workbook.Save("FolderFontSourceDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FolderFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


