---
title: "LightCellsDataHandler.StartCell"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة LightCellsDataHandler. تُحضّر لمعالجة خلية"
type: docs
url: /ar/net/aspose.cells/lightcellsdatahandler/startcell/
---
## LightCellsDataHandler.StartCell method

يجهز لمعالجة خلية.

```csharp
public bool StartCell(int columnIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | Int32 | فهرس العمود للخلية التي سيتم معالجتها |

### قيمة الإرجاع

ما إذا كانت هذه الخلية تحتاج إلى المعالجة. false لتجاهل الخلية والتحقق من التالية حتى الوصول إلى نهاية بيانات الخلايا للصف الحالي

### ملاحظات

سيتم استدعاؤها عند الوصول إلى خلية موجودة في الصف الحالي. الصف الحالي هو الصف الذي تم فيه آخر استدعاء لـ [`ProcessRow`](../processrow/).

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LightCellsDataHandlerMethodStartCellWithInt32Demo
    {
        public static void Run()
        {
            try
            {
                // إنشاء ملف إدخال مؤقت
                File.WriteAllText("input.csv", "Column1,Column2,Column3\n1,2,3\n4,5,6");

                // إنشاء خيارات التحميل مع معالج light cells مخصص
                LoadOptions loadOptions = new LoadOptions(LoadFormat.Csv);
                var handler = new CustomLightCellsDataHandler();
                loadOptions.LightCellsDataHandler = handler;

                // تحميل المصنف مع معالج مخصص
                Workbook workbook = new Workbook("input.csv", loadOptions);

                // حفظ المصنف المعالج
                workbook.Save("output.xlsx");
                Console.WriteLine("StartCell method executed successfully. Check output.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing StartCell method: {ex.Message}");
            }
        }

        private class CustomLightCellsDataHandler : LightCellsDataHandler
        {
            public bool StartSheet(Worksheet sheet)
            {
                return true; // Process all sheets
            }

            public bool StartRow(int rowIndex)
            {
                return true; // Process all rows
            }

            public bool StartCell(int columnIndex)
            {
                // معالجة الخلايا فقط في فهرس العمود 1 (العمود الثاني)
                return columnIndex == 1;
            }

            public bool ProcessCell(Cell cell)
            {
                // مضاعفة قيمة الخلايا في العمود الثاني
                if (cell.IsNumericValue)
                {
                    cell.PutValue(cell.DoubleValue * 2);
                }
                return true;
            }

            public bool ProcessRow(Row row)
            {
                return true; // Continue processing
            }
        }
    }
}
```

### انظر أيضًا

* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


