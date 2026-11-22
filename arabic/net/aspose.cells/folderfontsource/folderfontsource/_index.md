---
title: "FolderFontSource.FolderFontSource"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ FolderFontSource. Ctor"
type: docs
url: /ar/net/aspose.cells/folderfontsource/folderfontsource/
---
## FolderFontSource constructor

منشئ.

```csharp
public FolderFontSource(string folderPath, bool scanSubfolders)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| folderPath | String | مسار مجلد الخطوط |
| scanSubfolders | منطقي | يحدد ما إذا كان يجب مسح المجلدات الفرعية أم لا. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FolderFontSourceMethodCtorWithStringBooleanDemo
    {
        public static void Run()
        {
            string folderPath = @"C:\Fonts";
            bool scanSubfolders = true;
            FolderFontSource folderFontSource = new FolderFontSource(folderPath, scanSubfolders);

            Console.WriteLine("Folder Path: " + folderFontSource.FolderPath);
            Console.WriteLine("Scan Subfolders: " + folderFontSource.ScanSubFolders);

            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource });
            workbook.Save("FolderFontSourceExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FolderFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


