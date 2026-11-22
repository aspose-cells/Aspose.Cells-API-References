---
title: "الفئة CalculationOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.CalculationOptions. تمثل خيارات الحساب"
type: docs
url: /ar/net/aspose.cells/calculationoptions/
---
## CalculationOptions class

يمثل خيارات الحساب.

```csharp
public class CalculationOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [CalculationOptions](calculationoptions/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CalcStackSize](../../aspose.cells/calculationoptions/calcstacksize/) { get; set; } | حجم المكدس لحساب الخلايا بشكل متكرر. القيمة الافتراضية هي 200. |
| [CalculationMonitor](../../aspose.cells/calculationoptions/calculationmonitor/) { get; set; } | المراقب للمستخدم لتتبع تقدم حساب الصيغ. |
| [CharacterEncoding](../../aspose.cells/calculationoptions/characterencoding/) { get; set; } | يحدد الترميز المستخدم لترميز/فك ترميز الأحرف عند حساب الصيغ. بالنسبة للدوال مثل CHAR و CODE، تعتمد النتيجة المحسوبة على إعدادات المنطقة ومجموعة الأحرف الافتراضية للبيئة. باستخدام هذه الخاصية يمكن للمستخدم تحديد الترميز المناسب لتلك الدوال للحصول على النتيجة المتوقعة. |
| [CustomEngine](../../aspose.cells/calculationoptions/customengine/) { get; set; } | محرك حساب الصيغ المخصص لتوسيع محرك الحساب الافتراضي في Aspose.Cells. |
| [IgnoreError](../../aspose.cells/calculationoptions/ignoreerror/) { get; set; } | يشير إلى ما إذا كان يجب تجاهل الأخطاء التي تم مواجهتها أثناء حساب الصيغ. قد يكون الخطأ دالة غير مدعومة أو روابط خارجية، إلخ. القيمة الافتراضية هي true. |
| [LinkedDataSources](../../aspose.cells/calculationoptions/linkeddatasources/) { get; set; } | يحدد مصادر البيانات للروابط الخارجية المستخدمة في الصيغ. |
| [PrecisionStrategy](../../aspose.cells/calculationoptions/precisionstrategy/) { get; set; } | يحدد الاستراتيجية لمعالجة دقة الحساب. |
| [Recursive](../../aspose.cells/calculationoptions/recursive/) { get; set; } | يشير إلى ما إذا كان يتم حساب الخلايا التابعة بشكل متكرر عند حساب خلية واحدة وتعتمد على خلايا أخرى. القيمة الافتراضية هي true. |
| [RefreshDynamicArrayFormula](../../aspose.cells/calculationoptions/refreshdynamicarrayformula/) { get; set; } | يشير إلى ما إذا كان يجب تحديث صيغ المصفوفة الديناميكية قبل حساب الصيغ. |
| [UserSpecifiedRefreshDynamicArrayFormula](../../aspose.cells/calculationoptions/userspecifiedrefreshdynamicarrayformula/) { get; } | يشير إلى ما إذا كان المستخدم قد حدد صراحة سلوك تحديث صيغ المصفوفة الديناميكية قبل حساب الصيغ المحددة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Text;

    public class CalculationOptionsDemo
    {
        public static void CalculationOptionsExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            worksheet.Cells["A1"].PutValue(10.555);
            worksheet.Cells["A2"].PutValue(20.6666);
            worksheet.Cells["A3"].PutValue(30.7777);
            worksheet.Cells["A4"].Formula = "=SUM(A1:A3)";

            // إنشاء مثيل من CalculationOptions
            CalculationOptions calcOptions = new CalculationOptions
            {
                IgnoreError = true,
                Recursive = true,
                CalcStackSize = 200,
                PrecisionStrategy = CalculationPrecisionStrategy.Round,
                CharacterEncoding = Encoding.UTF8
            };

            // اختياريًا، يمكنك تعيين محرك حساب مخصص أو مراقب
            // calcOptions.CustomEngine = new MyCustomEngine();
            // calcOptions.CalculationMonitor = new MyCalculationMonitor();

            // احسب الصيغ في المصنف باستخدام الخيارات المحددة
            workbook.CalculateFormula(calcOptions);

            // احفظ المصنف
            workbook.Save("CalculationOptionsExample.xlsx");
            workbook.Save("CalculationOptionsExample.pdf");

        }
    }

    // مثال على محرك حساب مخصص (إذا لزم الأمر)
    public class MyCustomEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            // منطق حساب مخصص
            string funcName = data.FunctionName.ToUpper();
            if (funcName == "MYFUNC")
            {
                // مثال على منطق دالة مخصصة
                int count = data.ParamCount;
                object result = null;
                for (int i = 0; i < count; i++)
                {
                    object paramValue = data.GetParamValue(i);
                    if (paramValue is ReferredArea)
                    {
                        ReferredArea ra = (ReferredArea)paramValue;
                        paramValue = ra.GetValue(0, 0);
                    }
                    // معالجة المعامل هنا
                    // result = ...;
                }
                data.CalculatedValue = result;
            }
        }
    }

    // مثال على مراقب حساب مخصص (إذا لزم الأمر)
    public class MyCalculationMonitor : AbstractCalculationMonitor
    {
        public override void BeforeCalculate(int sheetIndex, int rowIndex, int colIndex)
        {
            // منطق قبل الحساب
            Console.WriteLine($"Before calculating cell at Sheet {sheetIndex}, Row {rowIndex}, Column {colIndex}");
        }

        public override void AfterCalculate(int sheetIndex, int rowIndex, int colIndex)
        {
            // منطق بعد الحساب
            Console.WriteLine($"After calculating cell at Sheet {sheetIndex}, Row {rowIndex}, Column {colIndex}");
        }

        public override bool OnCircular(System.Collections.IEnumerator circularCellsData)
        {
            // معالجة المراجع الدائرية
            Console.WriteLine("Circular reference detected.");
            return true; // Continue calculation
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


