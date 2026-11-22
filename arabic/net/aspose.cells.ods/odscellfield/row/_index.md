---
title: "OdsCellField.Row"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية OdsCellField. تحصل وتعيّن فهرس الصف للخلية"
type: docs
url: /ar/net/aspose.cells.ods/odscellfield/row/
---
## OdsCellField.Row property

يحصل على ويضبط فهرس الصف للخلية.

```csharp
public int Row { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsCellFieldPropertyRowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            OdsCellFieldCollection odsCellFields = worksheet.Cells.OdsCellFields;
            
            // أضف حقولًا بأنواع مختلفة
            odsCellFields.Add(0, 0, OdsCellFieldType.Date, "yyyy-mm-dd");
            odsCellFields.Add(1, 0, OdsCellFieldType.SheetName, null);
            odsCellFields.Add(2, 0, OdsCellFieldType.Title, null);
            
            odsCellFields.UpdateFieldsValue();

            // أظهر استخدام خاصية Row
            for (int i = 0; i < odsCellFields.Count; i++)
            {
                OdsCellField field = odsCellFields[i];
                int row = field.Row; // Using Row property
                worksheet.Cells[row, 1].PutValue($"Row: {row}, Type: {field.FieldType}");
            }

            workbook.Save("OdsCellFieldRowDemo.ods");
        }
    }
}
```

### انظر أيضًا

* class [OdsCellField](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


