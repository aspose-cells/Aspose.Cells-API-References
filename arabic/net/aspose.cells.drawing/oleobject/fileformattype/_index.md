---
title: "OleObject.FileFormatType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية OleObject. تحصل وتضبط نوع ملف بيانات كائن ole المضمّن"
type: docs
url: /ar/net/aspose.cells.drawing/oleobject/fileformattype/
---
## OleObject.FileFormatType property

يحصل على نوع الملف ويضبطه لبيانات كائن OLE المضمن

```csharp
public FileFormatType FileFormatType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyFileFormatTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف كائن OLE إلى ورقة العمل (بدون بيانات ملف)
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, null);
            
            // احصل على كائن OLE المضاف
            OleObject oleObject = worksheet.OleObjects[oleIndex];
            
            // قم بتعيين وعرض نوع تنسيق الملف
            oleObject.FileFormatType = FileFormatType.Docm;
            Console.WriteLine("OLE Object File Format Type: " + oleObject.FileFormatType);
            
            // احفظ المصنف
            workbook.Save("OleObjectFileFormatTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [FileFormatType](../../../aspose.cells/fileformattype/)
* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


