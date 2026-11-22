---
title: "الفئة FormulaSettings"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.FormulaSettings. إعدادات الصيغ والحساب"
type: docs
url: /ar/net/aspose.cells/formulasettings/
---
## FormulaSettings class

إعدادات الصيغ والحساب.

```csharp
public class FormulaSettings
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CalculateOnOpen](../../aspose.cells/formulasettings/calculateonopen/) { get; set; } | يشير إلى ما إذا كان التطبيق مطلوبًا لتنفيذ حساب كامل عند فتح المصنف. |
| [CalculateOnSave](../../aspose.cells/formulasettings/calculateonsave/) { get; set; } | يشير إلى ما إذا كان يجب إعادة حساب المصنف قبل حفظ المستند، عند وضع الحساب اليدوي. |
| [CalculationId](../../aspose.cells/formulasettings/calculationid/) { get; set; } | يحدد إصدار محرك الحساب المستخدم لحساب القيم في المصنف. |
| [CalculationMode](../../aspose.cells/formulasettings/calculationmode/) { get; set; } | يحصل أو يضبط وضع حساب المصنف في MS Excel. |
| [EnableCalculationChain](../../aspose.cells/formulasettings/enablecalculationchain/) { get; set; } | يشير إلى ما إذا كان يجب تمكين سلسلة الحساب للصيغ. القيمة الافتراضية هي false. |
| [EnableIterativeCalculation](../../aspose.cells/formulasettings/enableiterativecalculation/) { get; set; } | يشير إلى ما إذا كان يجب تمكين الحساب التكراري لحل المراجع الدائرية. |
| [ForceFullCalculation](../../aspose.cells/formulasettings/forcefullcalculation/) { get; set; } | يشير إلى ما إذا كان يحسب جميع الصيغ في كل مرة يتم فيها تشغيل حساب. |
| [MaxChange](../../aspose.cells/formulasettings/maxchange/) { get; set; } | الحد الأقصى للتغيير لحل مرجع دائري. |
| [MaxIteration](../../aspose.cells/formulasettings/maxiteration/) { get; set; } | الحد الأقصى للتكرارات لحل مرجع دائري. |
| [PrecisionAsDisplayed](../../aspose.cells/formulasettings/precisionasdisplayed/) { get; set; } | يشير إلى ما إذا كان يجب ضبط دقة النتيجة المحسوبة كما تُعرض أثناء حساب الصيغ. |
| [PreservePaddingSpaces](../../aspose.cells/formulasettings/preservepaddingspaces/) { get; set; } | يشير إلى ما إذا كان يجب الحفاظ على تلك الفراغات وفواصل الأسطر التي تُملأ بين رموز الصيغة أثناء الحصول على الصيغ وتعيينها. القيمة الافتراضية هي false. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormulaSettingsDemo
    {
        public static void FormulaSettingsExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى إعدادات صيغ المصنف
            FormulaSettings formulaSettings = workbook.Settings.FormulaSettings;

            // ضبط الخصائص
            formulaSettings.CalculateOnOpen = true;
            formulaSettings.CalculateOnSave = true;
            formulaSettings.ForceFullCalculation = false;
            formulaSettings.CalculationMode = CalcModeType.Automatic;
            formulaSettings.CalculationId = "0";
            formulaSettings.EnableIterativeCalculation = true;
            formulaSettings.MaxIteration = 100;
            formulaSettings.MaxChange = 0.001;
            formulaSettings.PrecisionAsDisplayed = false;
            formulaSettings.EnableCalculationChain = true;
            formulaSettings.PreservePaddingSpaces = false;

            // احفظ المصنف
            workbook.Save("FormulaSettingsExample.xlsx");
            workbook.Save("FormulaSettingsExample.pdf");
            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


