---
title: "ImportTableOptions.IsFieldNameShown"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImportTableOptions. تشير إلى ما إذا كان يجب استيراد اسم الحقل"
type: docs
url: /ar/net/aspose.cells/importtableoptions/isfieldnameshown/
---
## ImportTableOptions.IsFieldNameShown property

يشير إلى ما إذا كان يجب استيراد اسم الحقل.

```csharp
public bool IsFieldNameShown { get; set; }
```

### أمثلة

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyIsFieldNameShownDemo
    {
        public static void Run()
        {
            // أنشئ DataTable نموذجية
            DataTable table = new DataTable();
            table.Columns.Add("ID");
            table.Columns.Add("Product");
            
            // أضف بيانات تجريبية
            table.Rows.Add(1, "Laptop");
            table.Rows.Add(2, "Smartphone");
            table.Rows.Add(3, "Tablet");

            // إنشاء مصنف واستيراد البيانات مع إظهار أسماء الحقول
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            ImportTableOptions options = new ImportTableOptions();
            options.IsFieldNameShown = true;  // Show field names
            options.InsertRows = true;       // Insert new rows
            
            // استيراد البيانات بدءًا من الصف 5، العمود 0
            cells.ImportData(table, 5, 0, options);
            
            // احفظ المصنف
            workbook.Save("ImportDataWithFieldNames.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


