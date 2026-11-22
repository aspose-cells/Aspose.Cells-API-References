---
title: "TxtLoadOptions.TextQualifier"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TxtLoadOptions. تحدد محدد النص لقيم الخلايا. المحدد الافتراضي هو"
type: docs
url: /ar/net/aspose.cells/txtloadoptions/textqualifier/
---
## TxtLoadOptions.TextQualifier property

يحدد محدد النص لقيم الخلايا. المحدد الافتراضي هو '\"'.

```csharp
public char TextQualifier { get; set; }
```

### ملاحظات

عند ضبط هذه الخاصية، [`HasTextQualifier`](../hastextqualifier/) سيصبح true تلقائيًا.

### أمثلة

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyTextQualifierDemo
    {
        public static void Run()
        {
            // إنشاء مثال من TxtLoadOptions لملف CSV
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
            {
                Separator = ',',
                HasTextQualifier = true,
                TextQualifier = '\"'
            };

            // إنشاء بيانات CSV عينة مع محددات النص
            string csvData = "Name,Age,City\n\"John Doe\",30,\"New York\"\n\"Jane Smith\",25,\"San Francisco\"";
            
            // حفظ البيانات العينة إلى ملف مؤقت
            string tempFile = "temp.csv";
            System.IO.File.WriteAllText(tempFile, csvData);

            // تحميل ملف CSV بالخيارات المحددة
            Workbook workbook = new Workbook(tempFile, loadOptions);

            // حفظ المصنف إلى ملف Excel
            workbook.Save("TextQualifierDemo.xlsx");

            // تنظيف الملف المؤقت
            System.IO.File.Delete(tempFile);
        }
    }
}
```

### انظر أيضًا

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


