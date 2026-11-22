---
title: "OdsCellField.FieldType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية OdsCellField. تحصل وتضبط نوع الحقل"
type: docs
url: /ar/net/aspose.cells.ods/odscellfield/fieldtype/
---
## OdsCellField.FieldType property

يحصل على ويضبط نوع الحقل.

```csharp
public OdsCellFieldType FieldType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsCellFieldPropertyFieldTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة حقول خلايا ODS بأنواع حقول مختلفة وسلاسل تنسيق
            sheet.Cells.OdsCellFields.Add(0, 0, OdsCellFieldType.Title, "Title Format");
            sheet.Cells.OdsCellFields.Add(1, 0, OdsCellFieldType.SheetName, "SheetName Format");

            // إظهار استخدام خاصية FieldType
            Console.WriteLine("Field at (0,0) type: " + sheet.Cells.OdsCellFields[0].FieldType);
            Console.WriteLine("Field at (1,0) type: " + sheet.Cells.OdsCellFields[1].FieldType);

            // احفظ وأعد التحميل لإظهار الاستمرارية
            workbook.Save("output.ods");
            workbook = new Workbook("output.ods");
            sheet = workbook.Worksheets[0];

            // التحقق من FieldType بعد إعادة التحميل
            Console.WriteLine("After reload - Field at (0,0) type: " + sheet.Cells.OdsCellFields[0].FieldType);
            Console.WriteLine("After reload - Field at (1,0) type: " + sheet.Cells.OdsCellFields[1].FieldType);
        }
    }
}
```

### انظر أيضًا

* enum [OdsCellFieldType](../../odscellfieldtype/)
* class [OdsCellField](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


