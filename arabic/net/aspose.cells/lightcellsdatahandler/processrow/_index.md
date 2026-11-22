---
title: "LightCellsDataHandler.ProcessRow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة LightCellsDataHandler. يبدأ في معالجة صف واحد"
type: docs
url: /ar/net/aspose.cells/lightcellsdatahandler/processrow/
---
## LightCellsDataHandler.ProcessRow method

يبدأ معالجة صف واحد.

```csharp
public bool ProcessRow(Row row)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Row | كائن الصف الذي يتم معالجته حاليًا. |

### قيمة الإرجاع

ما إذا كانت خلايا هذا الصف تحتاج إلى المعالجة. false لتجاهل جميع الخلايا في هذا الصف.

### ملاحظات

سيتم استدعاؤه بعد قراءة خصائص الصف مثل الارتفاع، النمط، ... إلخ. ومع ذلك، لم يتم قراءة خلايا هذا الصف بعد.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataHandlerMethodProcessRowWithRowDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء دفتر عمل جديد
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // أضف بيانات تجريبية
                worksheet.Cells["A1"].Value = "Test Data";
                worksheet.Cells["A2"].Value = 100;
                worksheet.Cells["B2"].Value = 200;

                // إنشاء معالج مخصص
                var handler = new CustomRowHandler();

                // معالجة الصف الأول
                Row firstRow = worksheet.Cells.Rows[0];
                bool result = handler.ProcessRow(firstRow);

                Console.WriteLine($"ProcessRow returned: {result}");
                Console.WriteLine($"Row height after processing: {firstRow.Height}");

                workbook.Save("ProcessRowDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in ProcessRow demo: {ex.Message}");
            }
        }

        private class CustomRowHandler : LightCellsDataHandler
        {
            public bool ProcessRow(Row row)
            {
                // إظهار الوصول إلى خصائص الصف
                Console.WriteLine($"Processing row index: {row.Index}");
                Console.WriteLine($"Row is hidden: {row.IsHidden}");
                Console.WriteLine($"Row is blank: {row.IsBlank}");

                // تعديل ارتفاع الصف إذا لم يكن صف الرأس
                if (row.Index > 0)
                {
                    row.Height = 25.0;
                }

                return true;
            }

            public bool StartSheet(Worksheet sheet) => true;
            public bool StartRow(int rowIndex) => true;
            public bool StartCell(int columnIndex) => true;
            public bool ProcessCell(Cell cell) => true;
        }
    }
}
```

### انظر أيضًا

* class [Row](../../row/)
* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


