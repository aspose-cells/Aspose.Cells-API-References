---
title: "OleObject.IsLink"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية OleObject. تُرجع true إذا كان OleObject يرتبط بالملف"
type: docs
url: /ar/net/aspose.cells.drawing/oleobject/islink/
---
## OleObject.IsLink property

يرجع true إذا كان OleObject يرتبط بالملف.

```csharp
public bool IsLink { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyIsLinkDemo
    {
        public static void Run()
        {
            // تحميل دفتر العمل المصدر
            Workbook workbook = new Workbook("example.xlsm");

            // معالجة كل ورقة عمل
            foreach (Worksheet worksheet in workbook.Worksheets)
            {
                // معالجة كل كائن OLE في ورقة العمل
                foreach (Aspose.Cells.Drawing.OleObject ole in worksheet.OleObjects)
                {
                    // تجاوز إذا لم يكن كائن OLE مرتبطًا
                    if (!ole.IsLink)
                    {
                        Console.WriteLine("Skipping embedded OLE object");
                        continue;
                    }

                    // عرض وتعديل مسار الملف المرتبط
                    Console.WriteLine("Original linked file: " + ole.ObjectSourceFullName);
                    string newPath = ole.ObjectSourceFullName.Replace("C:", "D:");
                    ole.ObjectSourceFullName = newPath;
                    Console.WriteLine("Modified linked file: " + ole.ObjectSourceFullName);
                }
            }

            // احفظ المصنف المعدل
            workbook.Save("modified_example.xlsm");
            Console.WriteLine("File saved with updated OLE links.");
        }
    }
}
```

### انظر أيضًا

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


