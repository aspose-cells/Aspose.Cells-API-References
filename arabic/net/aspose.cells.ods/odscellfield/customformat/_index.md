---
title: "OdsCellField.CustomFormat"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية OdsCellField. تمثل التنسيق المخصص لقيمة الحقل"
type: docs
url: /ar/net/aspose.cells.ods/odscellfield/customformat/
---
## OdsCellField.CustomFormat property

يمثل التنسيق المخصص لقيمة الحقل.

```csharp
public string CustomFormat { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsCellFieldPropertyCustomFormatDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            OdsCellFieldCollection odsCellFields = worksheet.Cells.OdsCellFields;
            
            // حقل تاريخ بتنسيق مخصص
            odsCellFields.Add(0, 0, OdsCellFieldType.Date, "yyyy-mm-dd");
            
            // حقل اسم الورقة بدون تنسيق مخصص
            odsCellFields.Add(1, 0, OdsCellFieldType.SheetName, null);
            
            // حقل العنوان بتنسيق مخصص (يوضح تنسيق السلسلة)
            odsCellFields.Add(2, 0, OdsCellFieldType.Title, "Title Format: @");
            
            odsCellFields.UpdateFieldsValue();
            
            foreach (OdsCellField field in odsCellFields)
            {
                worksheet.Cells[field.Row, field.Column].PutValue(
                    $"Type: {field.FieldType}, Format: {field.CustomFormat ?? "None"}");
            }
            
            workbook.Save("OdsCellFieldCustomFormatDemo.ods");
        }
    }
}
```

### انظر أيضًا

* class [OdsCellField](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


