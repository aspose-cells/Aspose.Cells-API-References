---
title: "Cells.ImportDataView"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تستورد DataView إلى ورقة عمل"
type: docs
url: /ar/net/aspose.cells/cells/importdataview/
---
## Cells.ImportDataView method

يستورد DataView إلى ورقة عمل.

```csharp
public int ImportDataView(DataView dataView, int firstRow, int firstColumn)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| dataView | DataView | كائن DataView المراد استيراده. |
| firstRow | Int32 | رقم الصف للخلية الأولى التي سيتم الاستيراد فيها. |
| firstColumn | Int32 | رقم العمود للخلية الأولى التي سيتم الاستيراد فيها. |

### قيمة الإرجاع

إجمالي عدد الصفوف المستوردة

### أمثلة

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataViewWithDataViewInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // إنشاء DataTable نموذجي
            DataTable table = new DataTable("Products");
            table.Columns.Add("ID", typeof(int));
            table.Columns.Add("Name", typeof(string));
            table.Columns.Add("Price", typeof(decimal));

            // أضف بيانات تجريبية
            table.Rows.Add(1, "Laptop", 999.99m);
            table.Rows.Add(2, "Smartphone", 699.99m);
            table.Rows.Add(3, "Tablet", 399.99m);

            // إنشاء DataView من DataTable
            DataView dataView = new DataView(table);

            // استيراد DataView إلى ورقة العمل بدءًا من الصف 0، العمود 0
            cells.ImportDataView(dataView, 0, 0);

            // احفظ المصنف
            workbook.Save("ImportDataViewOutput.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


