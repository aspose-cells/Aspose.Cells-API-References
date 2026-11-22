---
title: "VbaModuleCollection.GetDesignerStorage"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة VbaModuleCollection. تمثل بيانات المصمم"
type: docs
url: /ar/net/aspose.cells.vba/vbamodulecollection/getdesignerstorage/
---
## VbaModuleCollection.GetDesignerStorage method

يمثل بيانات المصمم.

```csharp
public byte[] GetDesignerStorage(string name)
```

### ملاحظات

نحن لا ندعم تحليلها. فقط للنسخ.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModuleCollectionMethodGetDesignerStorageWithStringDemo
    {
        public static void Run()
        {
            // إنشاء مصنف مع مشروع VBA
            Workbook workbook = new Workbook();
            
            // إضافة وحدة مصمم
            int index = workbook.VbaProject.Modules.Add(VbaModuleType.Designer, "TestForm");
            
            // الحصول على تخزين المصمم (سيكون فارغًا في البداية)
            byte[] storage = workbook.VbaProject.Modules.GetDesignerStorage("TestForm");
            Console.WriteLine("Initial designer storage: " + (storage == null ? "null" : "exists"));
            
            // إضافة بعض بيانات تخزين المصمم
            byte[] sampleData = new byte[] { 0x01, 0x02, 0x03 };
            workbook.VbaProject.Modules.AddDesignerStorage("TestForm", sampleData);
            
            // الحصول على وعرض تخزين المصمم
            storage = workbook.VbaProject.Modules.GetDesignerStorage("TestForm");
            Console.WriteLine("Storage after adding: " + (storage == null ? "null" : BitConverter.ToString(storage)));
        }
    }
}
```

### انظر أيضًا

* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


