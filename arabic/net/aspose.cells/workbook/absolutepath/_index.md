---
title: "Workbook.AbsolutePath"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Workbook. تحصل وتضبط المسار المطلق للملف"
type: docs
url: /ar/net/aspose.cells/workbook/absolutepath/
---
## Workbook.AbsolutePath property

يحصل على ويضبط المسار المطلق للملف.

```csharp
public string AbsolutePath { get; set; }
```

### ملاحظات

يُستخدم فقط للروابط الخارجية.

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyAbsolutePathDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook sourceBook = new Workbook();
            
            // أضف بعض أوراق العمل
            sourceBook.Worksheets.Add("Sheet1");
            sourceBook.Worksheets.Add("Sheet2");

            // احفظ المصنف للحصول على مسار فعلي
            string sourcePath = Path.GetFullPath("output");
            if (!Directory.Exists(sourcePath))
            {
                Directory.CreateDirectory(sourcePath);
            }
            string sourceFilePath = Path.Combine(sourcePath, "example.xlsx");
            sourceBook.Save(sourceFilePath);

            // أعد فتح المصنف لتوضيح AbsolutePath
            Workbook reopenedBook = new Workbook(sourceFilePath);
            
            // استخدم خاصية AbsolutePath لإنشاء مسار كامل
            string pathToBook = Path.Combine(reopenedBook.AbsolutePath, reopenedBook.FileName);
            Console.WriteLine("Full path to workbook: " + pathToBook);

            // أضف روابط تشعبية باستخدام المسار
            SetHyperlink(reopenedBook.Worksheets[0], 0, pathToBook, reopenedBook.Worksheets[0].Name, "A1");
            SetHyperlink(reopenedBook.Worksheets[0], 1, pathToBook, reopenedBook.Worksheets[1].Name, "B1");

            // احفظ المصنف المعدل
            string destPath = Path.Combine(sourcePath, "modified_example.xlsx");
            reopenedBook.Save(destPath);
        }

        private static void SetHyperlink(Worksheet sheet, int linkIndex, string path, string sheetName, string cellRef)
        {
            HyperlinkCollection hyperlinks = sheet.Hyperlinks;
            hyperlinks.Add(cellRef, 1, 1, path + "#" + sheetName + "!A1");
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


