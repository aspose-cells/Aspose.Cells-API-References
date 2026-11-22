---
title: "SpreadsheetML2003SaveOptions.ExportColumnIndexOfCell"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SpreadsheetML2003SaveOptions. القيمة الافتراضية هي false مما يعني أنه سيتم تجاهل فهرس العمود إذا كانت الخلية متصلة بالخلية السابقة"
type: docs
url: /ar/net/aspose.cells/spreadsheetml2003saveoptions/exportcolumnindexofcell/
---
## SpreadsheetML2003SaveOptions.ExportColumnIndexOfCell property

القيمة الافتراضية هي false، وهذا يعني أنه سيتم تجاهل فهرس العمود إذا كانت الخلية متصلة بالخلية السابقة.

```csharp
public bool ExportColumnIndexOfCell { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpreadsheetML2003SaveOptionsPropertyExportColumnIndexOfCellDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية إلى الخلايا
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            
            // إنشاء خيارات الحفظ مع تمكين ExportColumnIndexOfCell
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions();
            saveOptions.ExportColumnIndexOfCell = true;
            
            // حفظ المصنف مع معلومات فهرس العمود
            workbook.Save("output_with_column_index.xml", saveOptions);
            
            Console.WriteLine("File saved with column index information.");
        }
    }
}
```

### انظر أيضًا

* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


