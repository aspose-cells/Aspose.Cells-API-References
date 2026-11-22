---
title: "واجهة LightCellsDataProvider"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "واجهة Aspose.Cells.LightCellsDataProvider. تمثل موفر بيانات لحفظ ملفات جداول البيانات الكبيرة في وضع الوزن الخفيف"
type: docs
url: /ar/net/aspose.cells/lightcellsdataprovider/
---
## LightCellsDataProvider interface

يمثل موفر البيانات لحفظ ملفات جداول البيانات الكبيرة في وضع خفيف الوزن.

```csharp
public interface LightCellsDataProvider
```

## الطرق

| الاسم | الوصف |
| --- | --- |
| [IsGatherString](../../aspose.cells/lightcellsdataprovider/isgatherstring/)() | يتحقق مما إذا كانت قيمة السلسلة الحالية للخلية تحتاج إلى جمعها في مجموعة عالمية. |
| [NextCell](../../aspose.cells/lightcellsdataprovider/nextcell/)() | يحصل على الخلية التالية التي سيتم حفظها. |
| [NextRow](../../aspose.cells/lightcellsdataprovider/nextrow/)() | يحصل على الصف التالي الذي سيتم حفظه. |
| [StartCell](../../aspose.cells/lightcellsdataprovider/startcell/)(Cell) | يبدأ بحفظ بيانات خلية واحدة. |
| [StartRow](../../aspose.cells/lightcellsdataprovider/startrow/)(Row) | يبدأ بحفظ بيانات صف واحد. |
| [StartSheet](../../aspose.cells/lightcellsdataprovider/startsheet/)(int) | يبدأ بحفظ ورقة عمل. |

### ملاحظات

عند حفظ مصنف باستخدام هذا الوضع، سيتم فحص [`StartSheet`](./startsheet/) عند حفظ كل ورقة عمل في المصنف. لورقة واحدة، إذا أعاد [`StartSheet`](./startsheet/) true، فسيتم توفير جميع البيانات والخصائص التي يجب حفظها للصفوف/الخلايا في هذه الورقة من خلال تنفيذ هذه الواجهة. في البداية، سيتم استدعاء [`NextRow`](./nextrow/) للحصول على فهرس الصف التالي الذي سيُحفظ. إذا تم إرجاع فهرس صف صالح (يجب أن يكون فهرس الصف بترتيب تصاعدي للصفوف التي سيتم حفظها)، فسيتم توفير كائن Row الذي يمثل هذا الصف بواسطة [`StartRow`](./startrow/) لتقوم التنفيذ بتعيين خصائصه. لصف واحد، سيتم فحص [`NextCell`](./nextcell/) أولاً. إذا تم إرجاع فهرس عمود صالح (يجب أن يكون فهرس العمود بترتيب تصاعدي لجميع خلايا الصف الحالي)، فسيتم توفير كائن Cell الذي يمثل هذه الخلية بواسطة [`StartCell`](./startcell/) لتقوم التنفيذ بتعيين بياناتها وخصائصها. بعد [`StartCell`](./startcell/) سيتم حفظ الخلية مباشرةً إلى ملف الجدول الناتج. ثم سيتم فحص الخلية التالية ومعالجتها. يرجى ملاحظة أنه يجب على المستخدم تحديث القيم والخصائص فقط لكائن Row/Cell الحالي الذي تم توفيره بواسطة الطريقة المقابلة. لأن بيانات الخلايا تُكتب إلى الملف الناتج بطريقة تدفقية، قد تكون معظم الكائنات الأخرى قد كُتبت بالفعل إلى الملف الناتج، أو تم جمع بعض البيانات العامة لها وكتابتها. لذلك عندما يقوم المستخدم بتحديث كائنات أخرى أثناء حفظ بيانات الخلايا، قد لا تؤثر تلك العمليات على البيانات المحفوظة. أو قد تتسبب، في أسوأ الأحوال، في حفظ بيانات غير متسقة إلى الملف الناتج مما يؤدي في النهاية إلى فساد الملف. لذا، بالنسبة لجميع الكائنات الأخرى مثل الأشكال، عرض الأعمدة والأنماط، التنسيقات الشرطية، ... إلخ، يرجى عدم التعامل معها في أي من طرق هذا التنفيذ. بدلاً من ذلك، يرجى إدارة هذه الكائنات وضبطها إلى الحالة النهائية قبل استدعاء طريقة "Save" للمصنف.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderDemo
    {
        public static void LightCellsDataProviderExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء LightCellsDataProvider مخصص
            CustomLightCellsDataProvider dataProvider = new CustomLightCellsDataProvider();

            // تعيين LightCellsDataProvider لحفظ المصنف
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsx)
            {
                LightCellsDataProvider = dataProvider
            };

            // حفظ المصنف باستخدام LightCellsDataProvider المخصص
            workbook.Save("LightCellsDataProviderExample.xlsx", saveOptions);
        }
    }

    public class CustomLightCellsDataProvider : LightCellsDataProvider
    {
        private int currentRow = -1;
        private int currentCell = -1;

        public bool StartSheet(int sheetIndex)
        {
            // ابدأ معالجة الورقة الأولى
            return sheetIndex == 0;
        }

        public int NextRow()
        {
            // انتقل إلى الصف التالي
            currentRow++;
            currentCell = -1;

            // إرجاع فهرس الصف الحالي أو -1 إذا لم يتبق صفوف
            return currentRow < 10 ? currentRow : -1;
        }

        public void StartRow(Row row)
        {
            // تهيئة الصف إذا لزم الأمر
        }

        public int NextCell()
        {
            // انتقل إلى الخلية التالية
            currentCell++;

            // إرجاع فهرس الخلية الحالية أو -1 إذا لم يتبق خلايا
            return currentCell < 10 ? currentCell : -1;
        }

        public void StartCell(Cell cell)
        {
            // تعيين قيمة الخلية
            cell.PutValue($"R{currentRow}C{currentCell}");
        }

        public bool IsGatherString()
        {
            // إرجاع ما إذا كان يجب جمع السلاسل في مجموعة عالمية
            return false;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


