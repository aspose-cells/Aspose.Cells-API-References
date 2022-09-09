---
title: SetDynamicArrayFormula
second_title: Aspose.Cells لمرجع .NET API
description: لتعيين صيغة الصفيف الديناميكي وجعل الصيغة تنتشر في الخلايا المجاورة إن أمكن.
type: docs
weight: 600
url: /ar/net/aspose.cells/cell/setdynamicarrayformula/
---
## SetDynamicArrayFormula(string, FormulaParseOptions, bool) {#setdynamicarrayformula}

لتعيين صيغة الصفيف الديناميكي وجعل الصيغة تنتشر في الخلايا المجاورة إن أمكن.

```csharp
public CellArea SetDynamicArrayFormula(string arrayFormula, FormulaParseOptions options, 
    bool calculateValue)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| arrayFormula | String | تعبير الصيغة |
| options | FormulaParseOptions | خيارات تحليل الصيغة. سيتم تجاهل خيار "التحليل" وسيتم دائمًا تحليل الصيغة فورًا |
| calculateValue | Boolean | سواء حساب صيغة الصفيف الديناميكية هذه لتلك الخلايا في النطاق الممتد. |

### قيمة الإرجاع

النطاق الذي يجب أن تمتد إليه الصيغة.

### أنظر أيضا

* struct [CellArea](../../cellarea)
* class [FormulaParseOptions](../../formulaparseoptions)
* class [Cell](../../cell)
* مساحة الاسم [Aspose.Cells](../../cell)
* المجسم [Aspose.Cells](../../../)

---

## SetDynamicArrayFormula(string, FormulaParseOptions, object[][], bool, bool) {#setdynamicarrayformula_1}

لتعيين صيغة الصفيف الديناميكي وجعل الصيغة تنتشر في الخلايا المجاورة إن أمكن.

```csharp
public CellArea SetDynamicArrayFormula(string arrayFormula, FormulaParseOptions options, 
    object[][] values, bool calculateRange, bool calculateValue)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| arrayFormula | String | تعبير الصيغة |
| options | FormulaParseOptions | خيارات تحليل الصيغة. سيتم تجاهل خيار "التحليل" وسيتم دائمًا تحليل الصيغة فورًا |
| values | Object[][] | قيم تلك الخلايا مع صيغة صفيف ديناميكية معينة |
| calculateRange | Boolean | ما إذا كان يتم حساب النطاق المسكوب لصيغة المصفوفة الديناميكية هذه. إذا لم تكن معلمة "القيم" خالية وكانت هذه العلامة خاطئة ، فسيكون ارتفاع النطاق المسكوب قيمًا ، وسيكون الطول والعرض قيمًا [0]. الطول. |
| calculateValue | Boolean | سواء كان حساب صيغة الصفيف الديناميكي هذه للخلايا الموجودة في النطاق المسكوب عندما تكون "القيم" فارغة أو أن العنصر المقابل في "القيم" لخلية واحدة فارغ . |

### قيمة الإرجاع

النطاق الذي يجب أن تمتد إليه الصيغة.

### أنظر أيضا

* struct [CellArea](../../cellarea)
* class [FormulaParseOptions](../../formulaparseoptions)
* class [Cell](../../cell)
* مساحة الاسم [Aspose.Cells](../../cell)
* المجسم [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->