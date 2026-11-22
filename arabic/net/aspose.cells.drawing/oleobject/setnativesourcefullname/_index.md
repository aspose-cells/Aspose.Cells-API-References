---
title: "OleObject.SetNativeSourceFullName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة OleObject. تُعيّن ole native source full file name مع المسار"
type: docs
url: /ar/net/aspose.cells.drawing/oleobject/setnativesourcefullname/
---
## OleObject.SetNativeSourceFullName method

يضبط الاسم الكامل للملف الأصلي لكائن OLE مع المسار.

```csharp
public void SetNativeSourceFullName(string sourceFullName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceFullName | String | الـ ole native source full file name |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class OleObjectMethodSetNativeSourceFullNameWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة OleObject إلى ورقة العمل
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0]); // Changed to empty byte array
            OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            try
            {
                // استدعِ طريقة SetNativeSourceFullName مع معامل من نوع string
                oleObject.SetNativeSourceFullName(@"C:\temp\updated_test.xlsx");
                
                Console.WriteLine("SetNativeSourceFullName method executed successfully with parameter: C:\\temp\\updated_test.xlsx");
                
                // اعرض التأثير عن طريق فحص خاصية ObjectSourceFullName
                Console.WriteLine($"OleObject's source is now: {oleObject.ObjectSourceFullName}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetNativeSourceFullName method: {ex.Message}");
            }
            
            // احفظ المصنف
            workbook.Save("OleObjectMethodSetNativeSourceFullNameDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


