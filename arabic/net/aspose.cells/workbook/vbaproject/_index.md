---
title: "Workbook.VbaProject"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Workbook. تحصل على VbaProject في جدول بيانات"
type: docs
url: /ar/net/aspose.cells/workbook/vbaproject/
---
## Workbook.VbaProject property

يحصل على `VbaProject` في جدول بيانات.

```csharp
public VbaProject VbaProject { get; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyVbaProjectDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى مشروع VBA (VbaProject للقراءة فقط، لا يمكننا سوى التحقق مما إذا كان موجودًا)
            if (workbook.VbaProject == null)
            {
                // إنشاء مشروع VBA عن طريق الحفظ كدفتر عمل يدعم الماكرو
                workbook.Save("temp.xlsm", SaveFormat.Xlsm);
                workbook = new Workbook("temp.xlsm");
                File.Delete("temp.xlsm");
            }

            // إضافة وحدة جديدة إلى مشروع VBA
            int moduleIndex = workbook.VbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
            
            // احصل على الوحدة المضافة وضع كودها
            VbaModule module = workbook.VbaProject.Modules[moduleIndex];
            module.Codes = "Sub Test()\r\n    MsgBox \"Hello from VBA!\"\r\nEnd Sub";

            // احفظ المصنف
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "VbaProjectDemo.xlsm");
            workbook.Save(outputPath, SaveFormat.Xlsm);
        }
    }
}
```

### انظر أيضًا

* class [VbaProject](../../../aspose.cells.vba/vbaproject/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


