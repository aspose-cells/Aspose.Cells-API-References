---
title: "LightCellsDataHandler.ProcessCell"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة LightCellsDataHandler. تبدأ بمعالجة خلية واحدة"
type: docs
url: /ar/net/aspose.cells/lightcellsdatahandler/processcell/
---
## LightCellsDataHandler.ProcessCell method

يبدأ معالجة خلية واحدة.

```csharp
public bool ProcessCell(Cell cell)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| خلية | خلية | كائن Cell الذي يتم معالجته حاليًا |

### قيمة الإرجاع

ما إذا كان يجب الاحتفاظ بهذه الخلية في نموذج cells model للورقة الحالية. عادةً يجب أن تكون false حتى لا يتم الاحتفاظ بجميع الخلايا في الذاكرة بعد معالجتها وبالتالي يتم توفير الذاكرة. لبعض الأغراض الخاصة مثل حاجة المستخدم للوصول إلى بعض الخلايا لاحقًا بعد معالجة المصنف بالكامل، يمكن للمستخدم جعل هذه الطريقة تُعيد true للاحتفاظ بتلك الخلايا الخاصة في نموذج Cells والوصول إليها لاحقًا عبر واجهات برمجة التطبيقات مثل Cells[row, column]. ومع ذلك، فإن الاحتفاظ ببيانات الخلايا في نموذج Cells سيتطلب المزيد من الذاكرة وإذا تم الاحتفاظ بجميع الخلايا فإن قراءة ملف القالب في وضع LightCells سيصبح مماثلًا لقراءته بالطريقة العادية.

### ملاحظات

سيتم استدعاؤها بعد قراءة بيانات خلية واحدة.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LightCellsDataHandlerMethodProcessCellWithCellDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء ملف بيانات مؤقت
                File.WriteAllText("input.txt", "A,B,C\n10,20,30\n40,50,60");

                // إنشاء خيارات التحميل مع معالج light cells مخصص
                LoadOptions loadOptions = new LoadOptions(LoadFormat.Csv);
                var handler = new CustomLightCellsDataHandler();
                loadOptions.LightCellsDataHandler = handler;

                // تحميل المصنف مع معالج مخصص
                Workbook workbook = new Workbook("input.txt", loadOptions);

                // حفظ النتائج المعالجة
                workbook.Save("output.xlsx");
                Console.WriteLine("ProcessCell executed successfully. Check output.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ProcessCell: {ex.Message}");
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
                return true; // Process all cells
            }

            public bool ProcessCell(Cell cell)
            {
                // مضاعفة القيم العددية ووضع علامة على السلاسل
                if (cell.IsNumericValue)
                {
                    cell.PutValue(cell.DoubleValue * 2);
                }
                else if (cell.Type == CellValueType.IsString)
                {
                    cell.PutValue($"TEXT: {cell.StringValue}");
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

* class [Cell](../../cell/)
* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


