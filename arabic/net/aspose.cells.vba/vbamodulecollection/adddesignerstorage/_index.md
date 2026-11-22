---
title: "VbaModuleCollection.AddDesignerStorage"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة VbaModuleCollection."
type: docs
url: /ar/net/aspose.cells.vba/vbamodulecollection/adddesignerstorage/
---
## VbaModuleCollection.AddDesignerStorage method

```csharp
public void AddDesignerStorage(string name, byte[] data)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String |  |
| بيانات | Byte[] |  |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;
    using System.Text;

    public class VbaModuleCollectionMethodAddDesignerStorageWithStringByteDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى مشروع VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            // تحضير البيانات لتخزين المصمم
            string storageName = "MyDesignerStorage";
            byte[] storageData = Encoding.UTF8.GetBytes("This is designer storage data");
            
            try
            {
                // استدعاء طريقة AddDesignerStorage
                vbaProject.Modules.AddDesignerStorage(storageName, storageData);
                
                Console.WriteLine("Designer storage added successfully");
                
                // تحقق من أن التخزين قد تم إضافته
                byte[] retrievedData = vbaProject.Modules.GetDesignerStorage(storageName);
                if (retrievedData != null)
                {
                    Console.WriteLine("Retrieved storage data: " + Encoding.UTF8.GetString(retrievedData));
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddDesignerStorage method: {ex.Message}");
            }
            
            // احفظ المصنف
            workbook.Save("VbaModuleCollectionMethodAddDesignerStorageWithStringByteDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


