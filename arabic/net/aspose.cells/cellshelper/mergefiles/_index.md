---
title: "CellsHelper.MergeFiles"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة CellsHelper. دمج بعض ملفات xls الكبيرة إلى ملف xls واحد"
type: docs
url: /ar/net/aspose.cells/cellshelper/mergefiles/
---
## CellsHelper.MergeFiles method

يدمج بعض ملفات xls الكبيرة إلى ملف xls واحد.

```csharp
public static void MergeFiles(string[] files, string cachedFile, string destFile)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| ملفات | String[] | الملفات. |
| cachedFile | String | ملف التخزين المؤقت. |
| destFile | String | ملف الوجهة. |

### ملاحظات

هذه الطريقة تدعم فقط دمج البيانات والأنماط والصيغ إلى الملف الجديد. يُستخدم ملف التخزين المؤقت لتخزين بعض البيانات المؤقتة.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsHelperMethodMergeFilesWithStringStringDemo
    {
        public static void Run()
        {
            // إنشاء ملفات Excel مؤقتة للدمج
            string[] filesToMerge = new string[2];
            filesToMerge[0] = "File1.xlsx";
            filesToMerge[1] = "File2.xlsx";

            // إنشاء دفاتر عمل نموذجية
            Workbook workbook1 = new Workbook();
            workbook1.Worksheets[0].Cells["A1"].PutValue("File 1 Content");
            workbook1.Save(filesToMerge[0]);

            Workbook workbook2 = new Workbook();
            workbook2.Worksheets[0].Cells["A1"].PutValue("File 2 Content");
            workbook2.Save(filesToMerge[1]);

            string cachedFile = "CacheFile.tmp";
            string outputFile = "MergedOutput.xlsx";

            try
            {
                // استدعاء MergeFiles مع معلمات String[]، String، String
                CellsHelper.MergeFiles(filesToMerge, cachedFile, outputFile);

                Console.WriteLine("Files merged successfully. Output saved to: " + outputFile);

                // تحقق من الملف المدمج
                Workbook mergedWorkbook = new Workbook(outputFile);
                Console.WriteLine("Merged content:");
                Console.WriteLine(mergedWorkbook.Worksheets[0].Cells["A1"].StringValue);
                Console.WriteLine(mergedWorkbook.Worksheets[1].Cells["A1"].StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error merging files: {ex.Message}");
            }
            finally
            {
                // تنظيف الملفات المؤقتة
                if (File.Exists(filesToMerge[0])) File.Delete(filesToMerge[0]);
                if (File.Exists(filesToMerge[1])) File.Delete(filesToMerge[1]);
                if (File.Exists(cachedFile)) File.Delete(cachedFile);
            }
        }
    }
}
```

### انظر أيضًا

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


