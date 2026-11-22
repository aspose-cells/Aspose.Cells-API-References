---
title: "VbaModuleCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية VbaModuleCollection. يحصل على VbaModule في القائمة حسب الفهرس"
type: docs
url: /ar/net/aspose.cells.vba/vbamodulecollection/item/
---
## VbaModuleCollection indexer (1 of 2)

يحصل على [`VbaModule`](../../vbamodule/) في القائمة حسب الفهرس.

```csharp
public VbaModule this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModuleCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // إنشاء مصنف جديد مع مشروع VBA
            Workbook workbook = new Workbook("sample.xlsm");
            
            // الحصول على مشروع VBA الموجود (VbaProject للقراءة فقط)
            VbaProject vbaProject = workbook.VbaProject;
            
            // إضافة وحدة إلى مشروع VBA
            int index = vbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
            
            // الوصول إلى الوحدة باستخدام خاصية Item
            VbaModule module = vbaProject.Modules[index];
            
            // إضافة بعض كود VBA إلى الوحدة
            module.Codes = "Sub TestMacro()\n    MsgBox \"Hello from VBA!\"\nEnd Sub";
            
            // احفظ المصنف
            workbook.Save("VbaModuleDemo.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### انظر أيضًا

* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)

---

## VbaModuleCollection indexer (2 of 2)

يحصل على [`VbaModule`](../../vbamodule/) في القائمة حسب الاسم.

```csharp
public VbaModule this[string name] { get; }
```

| معامل | الوصف |
| --- | --- |
| name | اسم الوحدة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModuleCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // أضف ورقة عمل
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة وحدة VBA إلى المصنف
            int moduleIndex = workbook.VbaProject.Modules.Add(worksheet);
            
            // الوصول إلى الوحدة باستخدام خاصية Item حسب الاسم
            VbaModule module = workbook.VbaProject.Modules[worksheet.CodeName];
            
            // تعيين شيفرة VBA
            module.Codes = "Sub Test()\r\n    MsgBox \"Hello World!\"\r\nEnd Sub";
            
            // احفظ المصنف
            workbook.Save("output.xlsm", SaveFormat.Xlsm);
            
            // تحقق عن طريق إعادة التحميل
            Workbook verifyWorkbook = new Workbook("output.xlsm");
            VbaModule verifyModule = verifyWorkbook.VbaProject.Modules[worksheet.CodeName];
            
            Console.WriteLine("VBA Code in saved file:");
            Console.WriteLine(verifyModule.Codes);
        }
    }
}
```

### انظر أيضًا

* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


