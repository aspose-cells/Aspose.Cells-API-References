---
title: "FileFormatUtil.DetectFileFormat"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة FileFormatUtil. يكتشف ويعيد المعلومات حول تنسيق ملف Excel المخزن في تدفق"
type: docs
url: /ar/net/aspose.cells/fileformatutil/detectfileformat/
---
## DetectFileFormat(Stream) {#detectfileformat}

يكشف ويعيد المعلومات حول تنسيق ملف إكسل المخزن في تدفق.

```csharp
public static FileFormatInfo DetectFileFormat(Stream stream)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| تدفق | Stream |  |

### قيمة الإرجاع

كائن [`FileFormatInfo`](../../fileformatinfo/) يحتوي على المعلومات المكتشفة.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class FileFormatUtilMethodDetectFileFormatWithStreamDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // جهّز MemoryStream ببيانات دفتر العمل
            using (MemoryStream stream = new MemoryStream())
            {
                // احفظ دفتر العمل إلى التدفق بصيغة XLSX
                workbook.Save(stream, SaveFormat.Xlsx);
                stream.Seek(0, SeekOrigin.Begin); // Reset stream position

                try
                {
                    // اكتشف تنسيق الملف من التدفق
                    FileFormatInfo fileFormatInfo = FileFormatUtil.DetectFileFormat(stream);
                    
                    // اعرض نتائج الكشف
                    Console.WriteLine($"Detected File Format Type: {fileFormatInfo.FileFormatType}");
                    Console.WriteLine($"Is Encrypted: {fileFormatInfo.IsEncrypted}");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error detecting file format: {ex.Message}");
                }
            }

            // احفظ دفتر العمل الأصلي للتحقق
            workbook.Save("DetectFileFormatWithStreamDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DetectFileFormat(Stream, string) {#detectfileformat_1}

يكشف ويعيد المعلومات حول تنسيق ملف إكسل المخزن في تدفق.

```csharp
public static FileFormatInfo DetectFileFormat(Stream stream, string password)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| تدفق | Stream |  |
| كلمة المرور | String | كلمة المرور للملفات ooxml المشفرة. |

### قيمة الإرجاع

كائن [`FileFormatInfo`](../../fileformatinfo/) يحتوي على المعلومات المكتشفة.

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodDetectFileFormatWithStreamStringDemo
    {
        public static void Run()
        {
            string sourcePath = "example.xlsx";
            
            using (Stream stream = File.OpenRead(sourcePath))
            {
                FileFormatInfo info = FileFormatUtil.DetectFileFormat(stream, "test");
                Console.WriteLine("File format: " + info.FileFormatType);
                Console.WriteLine("Is encrypted: " + info.IsEncrypted);
                Console.WriteLine("Is password valid: " + FileFormatUtil.VerifyPassword(stream, "test"));
            }

            using (Stream stream = File.OpenRead(sourcePath))
            {
                FileFormatInfo info = FileFormatUtil.DetectFileFormat(stream, "1234");
                Console.WriteLine("File format: " + info.FileFormatType);
                Console.WriteLine("Is encrypted: " + info.IsEncrypted);
            }
        }
    }
}
```

### انظر أيضًا

* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DetectFileFormat(string) {#detectfileformat_2}

يكشف ويعيد المعلومات حول تنسيق ملف إكسل المخزن في ملف.

```csharp
public static FileFormatInfo DetectFileFormat(string filePath)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| filePath | String | مسار الملف. |

### قيمة الإرجاع

كائن [`FileFormatInfo`](../../fileformatinfo/) يحتوي على المعلومات المكتشفة.

### ملاحظات

يدعم فقط فحص بعض الملفات ذات التوقيع السحري. إذا لم يكن هناك توقيع سحري، لا يمكننا اكتشاف تنسيق الملف بدقة.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodDetectFileFormatWithStringDemo
    {
        public static void Run()
        {
            string filePath = "example.xlsx";
            FileFormatInfo info = FileFormatUtil.DetectFileFormat(filePath);
            
            Console.WriteLine("Load Format: " + info.LoadFormat);
            Console.WriteLine("File Format Type: " + info.FileFormatType);
            
            SaveFormat saveFormat = FileFormatUtil.FileFormatToSaveFormat(info.FileFormatType);
            LoadFormat loadFormat = FileFormatUtil.SaveFormatToLoadFormat(saveFormat);
            
            Console.WriteLine("Save Format: " + saveFormat);
            Console.WriteLine("Load Format (converted): " + loadFormat);
        }
    }
}
```

### انظر أيضًا

* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DetectFileFormat(string, string) {#detectfileformat_3}

يكشف ويعيد المعلومات حول تنسيق ملف إكسل المخزن في ملف.

```csharp
public static FileFormatInfo DetectFileFormat(string filePath, string password)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| filePath | String | مسار الملف. |
| كلمة المرور | String | كلمة المرور للملفات ooxml المشفرة. |

### قيمة الإرجاع

كائن [`FileFormatInfo`](../../fileformatinfo/) يحتوي على المعلومات المكتشفة.

### ملاحظات

يدعم فقط فحص بعض الملفات ذات التوقيع السحري. إذا لم يكن هناك توقيع سحري، لا يمكننا اكتشاف تنسيق الملف بدقة.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodDetectFileFormatWithStringStringDemo
    {
        public static void Run()
        {
            string sourcePath = @"..\..\..\Data\";
            
            // اكتشف تنسيق ملف XLSX
            FileFormatInfo xlsxInfo = FileFormatUtil.DetectFileFormat(sourcePath + "example.xlsx", "password");
            Console.WriteLine("XLSX format: " + xlsxInfo.FileFormatType);

            // اكتشف تنسيق ملف DOCX
            FileFormatInfo docxInfo = FileFormatUtil.DetectFileFormat(sourcePath + "example.docx", "password");
            Console.WriteLine("DOCX format: " + docxInfo.FileFormatType);
        }
    }
}
```

### انظر أيضًا

* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


