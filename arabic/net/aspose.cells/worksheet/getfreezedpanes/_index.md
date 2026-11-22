---
title: "Worksheet.GetFreezedPanes"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Worksheet. تحصل على تجميد الألواح"
type: docs
url: /ar/net/aspose.cells/worksheet/getfreezedpanes/
---
## Worksheet.GetFreezedPanes method

يحصل على تجميد الألواح.

```csharp
public bool GetFreezedPanes(out int row, out int column, out int freezedRows, 
    out int freezedColumns)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32& | فهرس الصف. |
| عمود | Int32& | فهرس العمود. |
| freezedRows | Int32& | عدد الصفوف الظاهرة في اللوحة العلوية، لا يزيد عن فهرس الصف. |
| freezedColumns | Int32& | عدد الأعمدة الظاهرة في اللوحة اليسرى، لا يزيد عن فهرس العمود. |

### قيمة الإرجاع

إرجاع ما إذا كانت الورقة مجمدة

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodGetFreezedPanesWithInt32ParametersDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تجميد الألواح عند الخلية C5 (الصف 4، العمود 2) مع صفين مجمدين وعمود واحد مجمد
            worksheet.FreezePanes(4, 2, 2, 1);

            // إعلان المتغيرات لتخزين معلومات تجميد الألواح
            int row = 0;
            int column = 0;
            int freezedRows = 0;
            int freezedColumns = 0;

            try
            {
                // استدعاء طريقة GetFreezedPanes مع معلمات out
                bool hasFreeze = worksheet.GetFreezedPanes(out row, out column, out freezedRows, out freezedColumns);

                // عرض النتائج
                Console.WriteLine("Worksheet has freeze panes: " + hasFreeze);
                if (hasFreeze)
                {
                    Console.WriteLine("Freeze position - Row: " + row + ", Column: " + column);
                    Console.WriteLine("Frozen rows: " + freezedRows + ", Frozen columns: " + freezedColumns);
                }

                // احفظ المصنف
                workbook.Save("WorksheetMethodGetFreezedPanesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFreezedPanes method: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


