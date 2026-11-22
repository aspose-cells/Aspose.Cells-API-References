---
title: "OdsCellFieldCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة OdsCellFieldCollection. تضيف حقلًا"
type: docs
url: /ar/net/aspose.cells.ods/odscellfieldcollection/add/
---
## OdsCellFieldCollection.Add method

يضيف حقلًا.

```csharp
public int Add(int row, int column, OdsCellFieldType fieldType, string format)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف. |
| عمود | Int32 | فهرس العمود. |
| fieldType | OdsCellFieldType | نوع الحقل. |
| تنسيق | String | تنسيق الرقم للحقل. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsCellFieldCollectionMethodAddWithInt32Int32OdsCellFieldTypStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            OdsCellFieldCollection odsCellFields = worksheet.Cells.OdsCellFields;

            // إضافة أنواع مختلفة من الحقول
            odsCellFields.Add(0, 0, OdsCellFieldType.Date, "yyyy-MM-dd");
            odsCellFields.Add(1, 1, OdsCellFieldType.SheetName, null);
            odsCellFields.Add(2, 2, OdsCellFieldType.Title, "SampleTitle");

            odsCellFields.UpdateFieldsValue();
            workbook.Save("OdsCellFieldsDemo.ods");
        }
    }
}
```

### انظر أيضًا

* enum [OdsCellFieldType](../../odscellfieldtype/)
* class [OdsCellFieldCollection](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


