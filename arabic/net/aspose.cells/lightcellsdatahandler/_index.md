---
title: "الواجهة LightCellsDataHandler"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "واجهة Aspose.Cells.LightCellsDataHandler. تمثل معالج بيانات الخلايا لقراءة ملفات جداول البيانات الكبيرة في وضع الوزن الخفيف."
type: docs
url: /ar/net/aspose.cells/lightcellsdatahandler/
---
## LightCellsDataHandler interface

يمثل معالج بيانات الخلايا لقراءة ملفات جداول البيانات الكبيرة في وضع خفيف الوزن.

```csharp
public interface LightCellsDataHandler
```

## الطرق

| الاسم | الوصف |
| --- | --- |
| [ProcessCell](../../aspose.cells/lightcellsdatahandler/processcell/)(Cell) | يبدأ معالجة خلية واحدة. |
| [ProcessRow](../../aspose.cells/lightcellsdatahandler/processrow/)(Row) | يبدأ معالجة صف واحد. |
| [StartCell](../../aspose.cells/lightcellsdatahandler/startcell/)(int) | يجهز لمعالجة خلية. |
| [StartRow](../../aspose.cells/lightcellsdatahandler/startrow/)(int) | يجهز لمعالجة صف. |
| [StartSheet](../../aspose.cells/lightcellsdatahandler/startsheet/)(Worksheet) | يبدأ معالجة ورقة عمل. |

### ملاحظات

عند قراءة مصنف باستخدام هذا الوضع، سيتم فحص [`StartSheet`](./startsheet/) عند قراءة كل ورقة عمل في المصنف. لورقة واحدة، إذا أعاد [`StartSheet`](./startsheet/) true، فسيتم فحص جميع البيانات وخصائص الصفوف/الخلايا في هذه الورقة ومعالجتها بواسطة تنفيذ هذه الواجهة. لكل صف، سيتم استدعاء [`StartRow`](./startrow/) للتحقق مما إذا كان يحتاج إلى المعالجة. إذا كان الصف يحتاج إلى المعالجة، ستُقرأ خصائص هذا الصف أولاً ويمكن للمستخدم الوصول إلى خصائصه عبر [`ProcessRow`](./processrow/). إذا كانت خلايا الصف تحتاج إلى المعالجة أيضًا، يجب أن تُعيد [`ProcessRow`](./processrow/) true ثم يتم استدعاء [`StartCell`](./startcell/) لكل خلية موجودة في هذا الصف للتحقق مما إذا كانت الخلية تحتاج إلى المعالجة. إذا كانت الخلية تحتاج إلى المعالجة، سيتم استدعاء [`ProcessCell`](./processcell/) لمعالجة الخلية بواسطة تنفيذ هذه الواجهة. يرجى ملاحظة أنه يجب على المستخدم التعامل فقط مع القيم وخصائص كائن الصف/الخلية الحالي المقدم عبر الطريقة المقابلة. لأن بيانات الخلايا تُقرأ من ملف القالب بطريقة تدفقية، قد يتم إعادة ضبط/تحديث معظم الكائنات الأخرى لاحقًا بعد تحميل بيانات الخلايا. لذلك عند قيام المستخدم بتشغيل كائنات أخرى في هذا التنفيذ، قد لا تؤثر تلك العمليات على الكائنات الموجودة في المصنف. أو قد تتسبب في بيانات غير متسقة في المصنف وتؤدي إلى مشكلة أو استثناء غير متوقع لاحقًا. لذا، بالنسبة لجميع الكائنات الأخرى مثل الأشكال، عرض الأعمدة والأنماط، التنسيقات الشرطية، ... إلخ، يرجى عدم التعامل معها في أي من طرق هذا التنفيذ. بدلاً من ذلك، يرجى إدارتها بعد إنشاء المصنف.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataHandlerDemo : LightCellsDataHandler
    {
        public static void LightCellsDataHandlerExample()
        {
            // إنشاء مصنف وتحميله باستخدام LightCellsDataHandler
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نسخة من LightCellsDataHandlerDemo
            LightCellsDataHandlerDemo handler = new LightCellsDataHandlerDemo();

            // تعيين LightCellsDataHandler للمصنف
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.LightCellsDataHandler = handler;

            // تحميل دفتر العمل باستخدام خيارات التحميل المحددة
            workbook = new Workbook("LargeFile_original.xlsx", loadOptions);

            // حفظ المصنف لتوضيح العملية
            workbook.Save("ProcessedLargeFile.xlsx");
        }

        // تنفيذ طريقة StartSheet
        public bool StartSheet(Worksheet sheet)
        {
            Console.WriteLine("Starting to process sheet: " + sheet.Name);
            return true; // Continue processing
        }

        // تنفيذ طريقة StartRow
        public bool StartRow(int rowIndex)
        {
            Console.WriteLine("Starting to process row: " + rowIndex);
            return true; // Continue processing
        }

        // تنفيذ طريقة ProcessRow
        public bool ProcessRow(Row row)
        {
            Console.WriteLine("Processing row: " + row.Index);
            return true; // Continue processing
        }

        // تنفيذ طريقة StartCell
        public bool StartCell(int columnIndex)
        {
            Console.WriteLine("Starting to process cell in column: " + columnIndex);
            return true; // Continue processing
        }

        // تنفيذ طريقة ProcessCell
        public bool ProcessCell(Cell cell)
        {
            Console.WriteLine("Processing cell: " + cell.Name + " with value: " + cell.StringValue);
            return true; // Continue processing
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


