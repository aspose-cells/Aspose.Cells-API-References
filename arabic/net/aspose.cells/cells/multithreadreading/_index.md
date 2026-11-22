---
title: "Cells.MultiThreadReading"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cells. تحصل أو تعين ما إذا كان نموذج بيانات الخلايا يجب أن يدعم القراءة المتعددة الخيوط. القيمة الافتراضية لهذه الخاصية هي false"
type: docs
url: /ar/net/aspose.cells/cells/multithreadreading/
---
## Cells.MultiThreadReading property

يحصل أو يعيّن ما إذا كان نموذج بيانات الخلايا يجب أن يدعم القراءة متعددة الخيوط. القيمة الافتراضية لهذه الخاصية هي false.

```csharp
public bool MultiThreadReading { get; set; }
```

### ملاحظات

إذا كان هناك عدة خيوط لقراءة كائنات Row/Cell في هذه المجموعة بشكل متزامن، يجب تعيين هذه الخاصية إلى true، وإلا قد يتم إنتاج نتيجة غير متوقعة. قد يؤدي دعم القراءة المتعددة الخيوط إلى تدهور الأداء عند الوصول إلى كائنات Row/Cell من هذه المجموعة. يرجى ملاحظة أن بعض الميزات لا يمكنها دعم القراءة المتعددة الخيوط، مثل تنسيق القيم (عن طريق [`StringValue`](../../cell/stringvalue/)، [`DisplayStringValue`](../../cell/displaystringvalue/)، إلخ). لذلك، حتى إذا تم تعيين هذه الخاصية إلى true، قد لا تزال تلك APIs تعطي نتائج غير متوقعة للقراءة المتعددة الخيوط.

### أمثلة

```csharp
using System;
using System.Threading;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMultiThreadReadingDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // تمكين القراءة المتعددة الخيوط
            cells.MultiThreadReading = true;

            // إعداد النمط للعمود الأول
            Style style = wb.CreateStyle();
            style.Custom = "yyyy-mm-dd";
            StyleFlag sf = new StyleFlag();
            sf.All = true;
            cells.Columns[0].ApplyStyle(style, sf);

            // املأ الخلايا ببيانات تجريبية
            int rowCount = 1000;
            for (int i = 0; i < rowCount; i++)
            {
                cells[i, 0].PutValue(DateTime.Now.AddDays(i).ToOADate());
            }

            // إنشاء خيوط لقراءة قيم الخلايا
            int threadCount = 5;
            int cellsPerThread = rowCount / threadCount;
            int[] finishedCount = new int[1];
            System.Text.StringBuilder errors = new System.Text.StringBuilder();

            for (int i = 0; i < threadCount; i++)
            {
                int start = i * cellsPerThread;
                int end = (i == threadCount - 1) ? rowCount : start + cellsPerThread;
                
                Thread t = new Thread(() => 
                {
                    try
                    {
                        for (int row = start; row < end; row++)
                        {
                            object value = cells[row, 0].Value;
                            Console.WriteLine($"Thread {Thread.CurrentThread.ManagedThreadId}: Cell[{row},0] = {value}");
                        }
                        Interlocked.Increment(ref finishedCount[0]);
                    }
                    catch (Exception ex)
                    {
                        lock (errors)
                        {
                            errors.AppendLine($"Thread {Thread.CurrentThread.ManagedThreadId} error: {ex.Message}");
                        }
                    }
                });
                t.Start();
            }

            // انتظر حتى يكتمل جميع الخيوط
            while (finishedCount[0] < threadCount)
            {
                Thread.Sleep(200);
            }

            if (errors.Length > 0)
            {
                Console.WriteLine("Errors occurred:");
                Console.WriteLine(errors.ToString());
            }
            else
            {
                Console.WriteLine("All threads completed successfully");
            }
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


