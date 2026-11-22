---
title: "الفئة FileFormatInfo"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.FileFormatInfo. تحتوي على البيانات التي تُرجعها طرق كشف تنسيق الملف في FileFormatUtil"
type: docs
url: /ar/net/aspose.cells/fileformatinfo/
---
## FileFormatInfo class

يحتوي على البيانات التي تُرجعها طرق اكتشاف تنسيق الملف في [`FileFormatUtil`](../fileformatutil/).

```csharp
public class FileFormatInfo
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [FileFormatInfo](fileformatinfo/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [FileFormatType](../../aspose.cells/fileformatinfo/fileformattype/) { get; } | يحصل على تنسيق الملف المكتشف. |
| [IsEncrypted](../../aspose.cells/fileformatinfo/isencrypted/) { get; } | يرجع true إذا كان المستند مشفرًا ويتطلب كلمة مرور للفتح. |
| [IsProtectedByRMS](../../aspose.cells/fileformatinfo/isprotectedbyrms/) { get; } | يشير إلى ما إذا كان الملف محميًا بواسطة Microsoft Rights Management Server. |
| [LoadFormat](../../aspose.cells/fileformatinfo/loadformat/) { get; } | يحصل على تنسيق التحميل المكتشف. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FileFormatInfoDemo
    {
        public static void FileFormatInfoExample()
        {
            // حمّل ملفًا تجريبيًا لاكتشاف تنسيقه
            string filePath = "sample.xlsx";
            FileFormatInfo fileInfo = FileFormatUtil.DetectFileFormat(filePath);

            // اعرض معلومات تنسيق الملف
            Console.WriteLine("File Format Information:");
            Console.WriteLine($"Is Protected By RMS: {fileInfo.IsProtectedByRMS}");
            Console.WriteLine($"Is Encrypted: {fileInfo.IsEncrypted}");
            Console.WriteLine($"File Format Type: {fileInfo.FileFormatType}");
            Console.WriteLine($"Load Format: {fileInfo.LoadFormat}");

            // احفظ المعلومات في ملف نصي
            string outputFilePath = "FileFormatInfo.txt";
            using (System.IO.StreamWriter writer = new System.IO.StreamWriter(outputFilePath))
            {
                writer.WriteLine("File Format Information:");
                writer.WriteLine($"Is Protected By RMS: {fileInfo.IsProtectedByRMS}");
                writer.WriteLine($"Is Encrypted: {fileInfo.IsEncrypted}");
                writer.WriteLine($"File Format Type: {fileInfo.FileFormatType}");
                writer.WriteLine($"Load Format: {fileInfo.LoadFormat}");
            }

            Console.WriteLine($"File format information saved to {outputFilePath}");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


