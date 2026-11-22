---
title: "VbaModuleCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة VbaModuleCollection. تضيف وحدة لورقة عمل"
type: docs
url: /ar/net/aspose.cells.vba/vbamodulecollection/add/
---
## Add(Worksheet) {#add_1}

يضيف وحدة لورقة عمل.

```csharp
public int Add(Worksheet sheet)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| ورقة | ورقة العمل | ورقة العمل |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaModuleCollectionMethodAddWithWorksheetDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة وحدة VBA مرتبطة بورقة العمل
            int moduleIndex = workbook.VbaProject.Modules.Add(worksheet);
            
            // إضافة بعض كود VBA إلى الوحدة
            string vbaCode = "Sub Test()\n    MsgBox \"Hello from VBA!\"\nEnd Sub";
            workbook.VbaProject.Modules[moduleIndex].Codes = vbaCode;
            
            // حفظ المصنف مع مشروع VBA
            workbook.Save("output.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)

---

## Add(VbaModuleType, string) {#add}

يضيف وحدة.

```csharp
public int Add(VbaModuleType type, string name)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | VbaModuleType | نوع الوحدة. |
| name | String | اسم الوحدة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModuleCollectionMethodAddWithVbaModuleTypeStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            VbaProject vbaProject = workbook.VbaProject;

            int index = vbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
            VbaModule module = vbaProject.Modules[index];
            module.Codes = "Sub Test()\r\nMsgBox \"Hello World\"\r\nEnd Sub";

            workbook.Save("VbaModuleAddExample.xlsm");
        }
    }
}
```

### انظر أيضًا

* enum [VbaModuleType](../../vbamoduletype/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


