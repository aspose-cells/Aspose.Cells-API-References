---
title: "الفئة FileFormatUtil"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.FileFormatUtil. توفر طرقًا مساعدة لتحويل تعداد تنسيقات الملفات إلى سلاسل أو امتدادات ملفات والعكس"
type: docs
url: /ar/net/aspose.cells/fileformatutil/
---
## FileFormatUtil class

يوفر طرقًا مساعدة لتحويل تعداد تنسيق الملفات إلى سلاسل أو امتدادات ملفات والعكس.

```csharp
public class FileFormatUtil
```

## الطرق

| الاسم | الوصف |
| --- | --- |
| static [DetectFileFormat](../../aspose.cells/fileformatutil/detectfileformat/#detectfileformat)(Stream) | يكشف ويعيد المعلومات حول تنسيق ملف إكسل المخزن في تدفق. |
| static [DetectFileFormat](../../aspose.cells/fileformatutil/detectfileformat/#detectfileformat_2)(string) | يكشف ويعيد المعلومات حول تنسيق ملف إكسل المخزن في ملف. |
| static [DetectFileFormat](../../aspose.cells/fileformatutil/detectfileformat/#detectfileformat_1)(Stream, string) | يكشف ويعيد المعلومات حول تنسيق ملف إكسل المخزن في تدفق. |
| static [DetectFileFormat](../../aspose.cells/fileformatutil/detectfileformat/#detectfileformat_3)(string, string) | يكشف ويعيد المعلومات حول تنسيق ملف إكسل المخزن في ملف. |
| static [ExtensionToSaveFormat](../../aspose.cells/fileformatutil/extensiontosaveformat/)(string) | يحول امتداد اسم الملف إلى قيمة SaveFormat. |
| static [FileFormatToSaveFormat](../../aspose.cells/fileformatutil/fileformattosaveformat/)(FileFormatType) | تحويل تنسيق الملف إلى تنسيق حفظ. |
| static [IsTemplateFormat](../../aspose.cells/fileformatutil/istemplateformat/)(string) | يرجع true إذا كان الامتداد .xlt أو .xltX أو .xltm أو .ots. |
| static [LoadFormatToExtension](../../aspose.cells/fileformatutil/loadformattoextension/)(LoadFormat) | يحول قيمة تعداد تنسيق التحميل إلى امتداد ملف. |
| static [LoadFormatToSaveFormat](../../aspose.cells/fileformatutil/loadformattosaveformat/)(LoadFormat) | يحول قيمة LoadFormat إلى قيمة SaveFormat إذا كان ذلك ممكنًا. |
| static [SaveFormatToExtension](../../aspose.cells/fileformatutil/saveformattoextension/)(SaveFormat) | يحول قيمة تعداد تنسيق الحفظ إلى امتداد ملف. |
| static [SaveFormatToLoadFormat](../../aspose.cells/fileformatutil/saveformattoloadformat/)(SaveFormat) | يحول قيمة SaveFormat إلى قيمة LoadFormat إذا كان ذلك ممكنًا. |
| static [VerifyPassword](../../aspose.cells/fileformatutil/verifypassword/)(Stream, string) | يكشف ويعيد المعلومات حول تنسيق ملف إكسل المخزن في تدفق. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFileFormatUtilDemo
    {
        public static void Run()
        {
            string filePath = "example.xlt";
            
            // اكتشف تنسيق الملف
            FileFormatInfo info = FileFormatUtil.DetectFileFormat(filePath);
            Console.WriteLine("Detected file format: " + info.FileFormatType);
            
            // تحقق من تنسيق الملف باستخدام Workbook
            Workbook workbook = new Workbook(filePath);
            Console.WriteLine("Workbook file format: " + workbook.FileFormat);
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


