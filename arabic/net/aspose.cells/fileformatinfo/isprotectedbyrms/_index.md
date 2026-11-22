---
title: "FileFormatInfo.IsProtectedByRMS"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FileFormatInfo. تشير إلى ما إذا كان الملف محميًا بواسطة خادم إدارة الحقوق من مايكروسوفت"
type: docs
url: /ar/net/aspose.cells/fileformatinfo/isprotectedbyrms/
---
## FileFormatInfo.IsProtectedByRMS property

يشير إلى ما إذا كان الملف محميًا بواسطة Microsoft Rights Management Server.

```csharp
public bool IsProtectedByRMS { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatInfoPropertyIsProtectedByRMSDemo
    {
        public static void Run()
        {
            // مثال 1: التحقق مما إذا كان ملف Excel المحمي بواسطة RMS محميًا
            FileFormatInfo info1 = FileFormatUtil.DetectFileFormat("DRMExcel_document.xls");
            Console.WriteLine("Is file protected by RMS: " + info1.IsProtectedByRMS);

            // مثال 2: تحقق مما إذا كان ملف Excel العادي محميًا
            FileFormatInfo info2 = FileFormatUtil.DetectFileFormat("upload_simple_1.xls");
            Console.WriteLine("Is file protected by RMS: " + info2.IsProtectedByRMS);
        }
    }
}
```

### انظر أيضًا

* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


