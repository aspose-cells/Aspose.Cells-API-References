---
title: "VbaModuleCollection.Remove"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة VbaModuleCollection. تزيل وحدة لورقة عمل"
type: docs
url: /ar/net/aspose.cells.vba/vbamodulecollection/remove/
---
## Remove(Worksheet) {#remove}

يزيل وحدة لورقة عمل.

```csharp
public void Remove(Worksheet sheet)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| ورقة | ورقة العمل | ورقة العمل |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaModuleCollectionMethodRemoveWithWorksheetDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة وحدة VBA إلى ورقة العمل
            int moduleIndex = workbook.VbaProject.Modules.Add(worksheet);
            
            // الحصول على مجموعة وحدات VBA
            VbaModuleCollection modules = workbook.VbaProject.Modules;
            
            try
            {
                // استدعاء طريقة Remove مع معامل ورقة العمل
                modules.Remove(worksheet);
                
                Console.WriteLine("VBA module removed successfully for the specified worksheet.");
                
                // تحقق من أن الوحدة قد أزيلت
                if (modules.Count == 0)
                {
                    Console.WriteLine("No VBA modules remain in the collection.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Remove method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("VbaModuleRemoveWithWorksheetDemo.xlsx");
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

## Remove(string) {#remove_1}

إزالة الوحدة بالاسم

```csharp
public void Remove(string name)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String |  |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModuleCollectionMethodRemoveWithStringDemo
    {
        public static void Run()
        {
            // إنشاء مصنف مع ماكرو
            Workbook workbook = new Workbook();
            
            // الوصول إلى مشروع VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            // إضافة وحدة جديدة
            int index = vbaProject.Modules.Add(VbaModuleType.Procedural, "TestModule");
            
            // إضافة بعض الشيفرة إلى الوحدة
            vbaProject.Modules[index].Codes = "Sub Test()\r\nMsgBox \"Hello World\"\r\nEnd Sub";
            
            // احفظ المصنف
            workbook.Save("output_with_module.xlsm");
            
            // إزالة الوحدة بالاسم
            vbaProject.Modules.Remove("TestModule");
            
            // حفظ المصنف بعد الإزالة
            workbook.Save("output_after_removal.xlsm");
        }
    }
}
```

### انظر أيضًا

* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


