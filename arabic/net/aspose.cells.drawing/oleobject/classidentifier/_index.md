---
title: "OleObject.ClassIdentifier"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية OleObject. تحصل وتعيّن معرف الفئة للكائن المدمج. يعني أي تطبيق يفتح الملف المدمج"
type: docs
url: /ar/net/aspose.cells.drawing/oleobject/classidentifier/
---
## OleObject.ClassIdentifier property

يحصل على معرف الفئة للكائن المضمّن ويضبطه. يعني ذلك أي تطبيق يفتح الملف المضمّن.

```csharp
public byte[] ClassIdentifier { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyClassIdentifierDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // مصفوفة بايت تجريبية لـ ClassIdentifier (عادةً ما تكون معرف فئة حقيقي)
            byte[] classId = new byte[] { 0x01, 0x02, 0x03, 0x04, 0x05, 0x06, 0x07, 0x08, 
                                         0x09, 0x0A, 0x0B, 0x0C, 0x0D, 0x0E, 0x0F, 0x10 };

            // إضافة كائن OLE ببيانات تجريبية
            int oleIndex = sheet.OleObjects.Add(10, 10, 200, 100, new byte[100]);
            OleObject oleObject = sheet.OleObjects[oleIndex];
            
            // تعيين خاصية ClassIdentifier
            oleObject.ClassIdentifier = classId;
            oleObject.ProgID = "Excel.Sheet.12";
            oleObject.DisplayAsIcon = true;

            // احفظ المصنف
            workbook.Save("OleObjectDemo.xlsx");

            // تحميل دفتر العمل المحفوظ للتحقق من ClassIdentifier
            Workbook loadedWorkbook = new Workbook("OleObjectDemo.xlsx");
            OleObject loadedOle = loadedWorkbook.Worksheets[0].OleObjects[0];
            
            // تحقق من أن ClassIdentifier تم حفظه
            Console.WriteLine("ClassIdentifier length: " + loadedOle.ClassIdentifier.Length);
        }
    }
}
```

### انظر أيضًا

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


