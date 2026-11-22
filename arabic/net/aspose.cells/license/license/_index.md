---
title: "License.License"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ License. يهيئ نسخة جديدة من هذه الفئة"
type: docs
url: /ar/net/aspose.cells/license/license/
---
## License constructor

يُنشئ مثيلًا جديدًا لهذه الفئة.

```csharp
public License()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LicenseMethodCtorDemo
    {
        public static void Run()
        {
            // أنشئ نسخة جديدة من License باستخدام المنشئ (#ctor)
            License license = new License();
            
            // حدد ملف الترخيص
            license.SetLicense("MyLicense.lic");
            
            Console.WriteLine("License set successfully.");
        }
    }
}
```

### انظر أيضًا

* class [License](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


