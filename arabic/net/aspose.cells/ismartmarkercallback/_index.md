---
title: "الواجهة ISmartMarkerCallBack"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "واجهة Aspose.Cells.ISmartMarkerCallBack. تمثل واجهة رد الاتصال لمعالجة العلامة الذكية"
type: docs
url: /ar/net/aspose.cells/ismartmarkercallback/
---
## ISmartMarkerCallBack interface

يمثل واجهة الاستدعاء لمعالجة smartmarker.

```csharp
public interface ISmartMarkerCallBack
```

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Process](../../aspose.cells/ismartmarkercallback/process/)(int, int, int, string, string) | رد اتصال لمعالجة علامة ذكية. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ISmartMarkerCallBackDemo : ISmartMarkerCallBack
    {
        // تنفيذ طريقة Process من واجهة ISmartMarkerCallBack
        public void Process(int sheetIndex, int rowIndex, int colIndex, string tableName, string columnName)
        {
            // مثال على تنفيذ طريقة Process
            Console.WriteLine($"Processing sheetIndex: {sheetIndex}, rowIndex: {rowIndex}, colIndex: {colIndex}, tableName: {tableName}, columnName: {columnName}");
        }

        public static void ISmartMarkerCallBackExample()
        {
            // إنشاء كائن WorkbookDesigner جديد
            WorkbookDesigner designer = new WorkbookDesigner();
            // فتح ملف قالب (يحتوي على علامات ذكية)
            designer.Workbook = new Workbook("ISmartMarkerCallBackExample_original.xlsx");

            // تعيين واجهة رد الاتصال
            designer.CallBack = new ISmartMarkerCallBackDemo();

            // تهيئة البيانات الخاصة بك من مصدر البيانات
            // للتوضيح، سنستخدم DataTable بسيط
            System.Data.DataTable dataTable = new System.Data.DataTable("Table1");
            dataTable.Columns.Add("Column1", typeof(string));
            dataTable.Rows.Add("Value1");
            dataTable.Rows.Add("Value2");

            // تعيين DataTable كمصدر للبيانات
            designer.SetDataSource(dataTable);

            // معالجة العلامات الذكية لملء البيانات في أوراق العمل
            designer.Process(true);

            // احفظ ملف Excel
            designer.Workbook.Save("ISmartMarkerCallBackExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


