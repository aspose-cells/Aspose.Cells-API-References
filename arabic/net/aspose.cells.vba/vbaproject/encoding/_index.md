---
title: "VbaProject.Encoding"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية VbaProject. تحصل وتضبط ترميز مشروع VBA"
type: docs
url: /ar/net/aspose.cells.vba/vbaproject/encoding/
---
## VbaProject.Encoding property

يحصل ويضبط ترميز مشروع VBA.

```csharp
public Encoding Encoding { get; set; }
```

### أمثلة

```csharp
using System;
using System.Text;
using Aspose.Cells;
using Aspose.Cells.Vba;
using System.Security.Cryptography.X509Certificates;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyEncodingDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // تهيئة مشروع VBA
            VbaProject vbaProject = workbook.VbaProject;

            // تعيين خصائص مشروع VBA بما في ذلك الترميز
            vbaProject.Name = "TestVbaProject";
            vbaProject.Encoding = Encoding.UTF8;

            // إضافة وحدة إلى مشروع VBA
            vbaProject.Modules.Add(VbaModuleType.Class, "TestModule");

            // حفظ المصنف مع مشروع VBA
            workbook.Save("VbaProjectEncodingDemo.xlsm");
        }
    }
}
```

### انظر أيضًا

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


