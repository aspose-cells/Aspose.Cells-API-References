---
title: "CellsHelper.LibraryPath"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CellsHelper. تحصل أو تعين مسار المكتبة الذي يُشار إليه من قبل بعض مراجع الصيغ الخارجية"
type: docs
url: /ar/net/aspose.cells/cellshelper/librarypath/
---
## CellsHelper.LibraryPath property

يحصل أو يعيّن مسار المكتبة الذي يُشار إليه من قبل بعض مراجع الصيغ الخارجية.

```csharp
public static string LibraryPath { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyLibraryPathDemo
    {
        public static void Run()
        {
            // عيّن خاصية LibraryPath
            CellsHelper.LibraryPath = "C:\\MyLibraries\\AsposeCells";

            // أظهر الحصول على مسار LibraryPath واستخدامه
            Console.WriteLine("Current Library Path: " + CellsHelper.LibraryPath);

            // مثال على استخدام المسار في عملية ملف
            string filePath = System.IO.Path.Combine(CellsHelper.LibraryPath, "test.xlsx");
            Console.WriteLine("Would load file from: " + filePath);
        }
    }
}
```

### انظر أيضًا

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


