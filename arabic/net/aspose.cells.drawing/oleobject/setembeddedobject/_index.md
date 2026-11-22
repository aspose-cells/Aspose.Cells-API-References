---
title: "OleObject.SetEmbeddedObject"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة OleObject. تقوم بتعيين بيانات الكائن المضمن"
type: docs
url: /ar/net/aspose.cells.drawing/oleobject/setembeddedobject/
---
## SetEmbeddedObject(bool, byte[], string, bool, string) {#setembeddedobject}

يضبط بيانات الكائن المضمن.

```csharp
public void SetEmbeddedObject(bool linkToFile, byte[] objectData, string sourceFileName, 
    bool displayAsIcon, string label)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| linkToFile | منطقي | يشير إلى ما إذا كان الكائن يرتبط بالملف. إذا كان true، يتم تجاهل المعامل objectData. |
| objectData | Byte[] | بيانات الكائن المضمن. |
| sourceFileName | String | اسم الملف. |
| displayAsIcon | منطقي | يشير إلى ما إذا كان يتم عرض الكائن كأيقونة. إذا كان true، سيتم تغطية بيانات الصورة الأصلية بالأيقونة. |
| label | String | تسمية الأيقونة. تعمل فقط عندما يكون displayAsIcon true. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class OleObjectMethodSetEmbeddedObjectWithBooleanByteArrayStringBooleanStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة OleObject إلى ورقة العمل
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0]);
            OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            try
            {
                // تحضير المعاملات لـ SetEmbeddedObject
                bool linkToFile = false;
                byte[] objectData = File.ReadAllBytes("sample.xlsx");
                string sourceFileName = "sample.xlsx";
                bool displayAsIcon = false;
                string label = "Excel Document";

                // استدعاء SetEmbeddedObject بالمعاملات المحددة
                oleObject.SetEmbeddedObject(linkToFile, objectData, sourceFileName, displayAsIcon, label);

                Console.WriteLine("SetEmbeddedObject executed successfully with parameters (Boolean, Byte[], String, Boolean, String)");
                
                // عرض بعض الخصائص لإظهار التأثير
                Console.WriteLine($"OleObject label: {oleObject.Label}");
                Console.WriteLine($"Display as icon: {oleObject.DisplayAsIcon}");
                Console.WriteLine($"Is linked to file: {oleObject.IsLink}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetEmbeddedObject method: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("OleObjectMethodSetEmbeddedObjectDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## SetEmbeddedObject(bool, byte[], string, bool, string, bool) {#setembeddedobject_1}

يضبط بيانات الكائن المضمن.

```csharp
public void SetEmbeddedObject(bool linkToFile, byte[] objectData, string sourceFileName, 
    bool displayAsIcon, string label, bool updateIcon)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| linkToFile | منطقي | يشير إلى ما إذا كان الكائن يرتبط بالملف. إذا كان true، يتم تجاهل المعامل objectData. |
| objectData | Byte[] | بيانات الكائن المضمن. |
| sourceFileName | String | اسم الملف. |
| displayAsIcon | منطقي | يشير إلى ما إذا كان يتم عرض الكائن كأيقونة. إذا كان true، سيتم تغطية بيانات الصورة الأصلية بالأيقونة. |
| label | String | تسمية الأيقونة. تعمل فقط عندما يكون displayAsIcon true. |
| updateIcon | منطقي | يشير إلى ما إذا كان يتم تحديث الأيقونة تلقائيًا. |

### ملاحظات

نظرًا لأن Aspose يمكنه تحديث جميع أيقونات الملفات المضمنة، فمن الأفضل أن تضيف الأيقونة الصحيحة مع *updateIcon* كقيمة false.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class OleObjectMethodSetEmbeddedObjectWithBooleanByteArrayStringBooleanStringBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة OleObject إلى ورقة العمل
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0]);
            OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            try
            {
                // تحضير المعاملات لـ SetEmbeddedObject
                bool linkToFile = false;
                byte[] objectData = File.ReadAllBytes("sample.docx");
                string sourceFileName = "sample.docx";
                bool displayAsIcon = true;
                string label = "Word Document";
                bool updateIcon = true;

                // استدعاء SetEmbeddedObject بالمعاملات المحددة
                oleObject.SetEmbeddedObject(linkToFile, objectData, sourceFileName, displayAsIcon, label, updateIcon);

                Console.WriteLine("SetEmbeddedObject executed successfully with parameters (Boolean, Byte[], String, Boolean, String, Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetEmbeddedObject method: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("OleObjectMethodSetEmbeddedObjectDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


