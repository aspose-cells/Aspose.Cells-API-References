---
title: "OleObject.Label"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية OleObject. تحصل وتضبط تسمية العرض للكائن ole المرتبط"
type: docs
url: /ar/net/aspose.cells.drawing/oleobject/label/
---
## OleObject.Label property

يحصل على تسمية العرض ويضبطها لكائن OLE المرتبط.

```csharp
public string Label { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyLabelDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف كائن OLE مع تسمية
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0]);
            OleObject oleObject = worksheet.OleObjects[oleIndex];
            oleObject.Label = "label_nameです";

            // احفظ وأعد تحميل المصنف
            string outputPath = "output.xlsx";
            workbook.Save(outputPath);
            
            // تحقق من خاصية label
            Workbook loadedWorkbook = new Workbook(outputPath);
            OleObject loadedOleObject = loadedWorkbook.Worksheets[0].OleObjects[0];
            Console.WriteLine("OLE Object Label: " + loadedOleObject.Label);
        }
    }
}
```

### انظر أيضًا

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


