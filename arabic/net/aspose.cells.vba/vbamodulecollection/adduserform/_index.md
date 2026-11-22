---
title: "VbaModuleCollection.AddUserForm"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة VbaModuleCollection. إدراج نموذج مستخدم في مشروع VBA"
type: docs
url: /ar/net/aspose.cells.vba/vbamodulecollection/adduserform/
---
## VbaModuleCollection.AddUserForm method

إدراج نموذج مستخدم في مشروع VBA.

```csharp
public int AddUserForm(string name, string codes, byte[] designerStorage)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم نموذج المستخدم |
| الأكواد | String | الأكواد الخاصة بنموذج المستخدم |
| designerStorage | Byte[] | إعدادات المصمم الخاصة بنموذج المستخدم |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;
    using System.IO;

    public class VbaModuleCollectionMethodAddUserFormWithStringStringByteDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى مشروع VBA
            VbaProject vbaProject = workbook.VbaProject;
            VbaModuleCollection vbaModules = vbaProject.Modules;

            // تحضير المعلمات لـ AddUserForm
            string formName = "UserForm1";
            string formCode = 
                "Private Sub CommandButton1_Click()\n" +
                "    MsgBox \"Hello from UserForm!\"\n" +
                "End Sub";
            
            // إنشاء تخزين مصمم بسيط (عادةً ما يكون هذا هو بيانات .frx الثنائية)
            byte[] designerStorage = new byte[] { 0x00, 0x01, 0x02, 0x03 };

            try
            {
                // استدعاء AddUserForm مع معلمات (String, String, Byte[])
                int moduleIndex = vbaModules.AddUserForm(formName, formCode, designerStorage);
                
                Console.WriteLine($"UserForm added successfully at index: {moduleIndex}");
                Console.WriteLine($"Total VBA modules: {vbaModules.Count}");

                // احفظ المصنف لرؤية تغييرات مشروع VBA
                workbook.Save("AddUserFormDemo.xlsm", SaveFormat.Xlsm);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding UserForm: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


