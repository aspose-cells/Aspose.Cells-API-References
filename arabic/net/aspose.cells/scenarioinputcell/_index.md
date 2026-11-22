---
title: "الفئة Aspose.Cells.ScenarioInputCell. تمثل خلية الإدخال للسيناريو"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.ScenarioInputCell. يمثل خلية الإدخال للسيناريو"
type: docs
url: /ar/net/aspose.cells/scenarioinputcell/
---
## ScenarioInputCell class

يمثل خلية الإدخال للسيناريو.

```csharp
public class ScenarioInputCell
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Column](../../aspose.cells/scenarioinputcell/column/) { get; } | يحصل على ويضبط فهرس العمود للخلية المدخلة. |
| [IsDeleted](../../aspose.cells/scenarioinputcell/isdeleted/) { get; set; } | يشير إلى ما إذا كانت الخلية المدخلة محذوفة. |
| [Name](../../aspose.cells/scenarioinputcell/name/) { get; } | يحصل على ويضبط عنوان الخلية المدخلة. |
| [Row](../../aspose.cells/scenarioinputcell/row/) { get; } | يحصل على ويضبط فهرس الصف للخلية المدخلة. |
| [Value](../../aspose.cells/scenarioinputcell/value/) { get; set; } | يحصل على ويضبط قيمة الخلية المدخلة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ScenarioInputCellDemo
    {
        public static void ScenarioInputCellExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة سيناريو إلى ورقة العمل
            int scenarioIndex = worksheet.Scenarios.Add("Scenario 1");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // إضافة خلايا الإدخال إلى السيناريو
            ScenarioInputCellCollection inputCells = scenario.InputCells;
            inputCells.Add(0, 0, "100"); // Adding cell A1 with value 100
            inputCells.Add(1, 1, "200"); // Adding cell B2 with value 200

            // الوصول إلى خلايا الإدخال
            ScenarioInputCell inputCell1 = inputCells[0];
            ScenarioInputCell inputCell2 = inputCells[1];

            // عرض خصائص خلايا الإدخال
            Console.WriteLine($"Input Cell 1: Row = {inputCell1.Row}, Column = {inputCell1.Column}, Value = {inputCell1.Value}, IsDeleted = {inputCell1.IsDeleted}");
            Console.WriteLine($"Input Cell 2: Row = {inputCell2.Row}, Column = {inputCell2.Column}, Value = {inputCell2.Value}, IsDeleted = {inputCell2.IsDeleted}");

            // تعديل قيمة الخلية المدخلة الأولى
            inputCell1.Value = "150";

            // احفظ المصنف
            workbook.Save("ScenarioInputCellExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


