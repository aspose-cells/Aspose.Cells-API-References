---
title: "Cells.ImportDataRow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تستورد DataRow إلى ملف Excel"
type: docs
url: /ar/net/aspose.cells/cells/importdatarow/
---
## Cells.ImportDataRow method

يستورد DataRow إلى ملف Excel.

```csharp
public void ImportDataRow(DataRow dataRow, int row, int firstColumn)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| dataRow | DataRow | كائن DataRow. |
| صف | Int32 | فهرس الصف. |
| firstColumn | Int32 | فهرس العمود الأول. |

### أمثلة

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataRowWithDataRowInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // أنشئ DataTable نموذجية
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));

            // أضف بيانات تجريبية
            dataTable.Rows.Add(1, "Product A", 19.99m);
            dataTable.Rows.Add(2, "Product B", 29.99m);

            // استيراد الصف الأول من DataTable إلى ورقة العمل بدءًا من الصف 0، العمود 0
            cells.ImportDataRow(dataTable.Rows[0], 0, 0);

            // احفظ المصنف
            workbook.Save("ImportDataRowDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


