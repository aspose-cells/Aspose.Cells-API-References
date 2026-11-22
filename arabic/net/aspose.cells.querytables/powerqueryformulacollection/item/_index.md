---
title: "PowerQueryFormulaCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PowerQueryFormulaCollection. تحصل على PowerQueryFormula حسب الفهرس في القائمة"
type: docs
url: /ar/net/aspose.cells.querytables/powerqueryformulacollection/item/
---
## PowerQueryFormulaCollection indexer (1 of 2)

يحصل على [`PowerQueryFormula`](../../powerqueryformula/) حسب الفهرس في القائمة.

```csharp
public PowerQueryFormula this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // احصل على صيغ Power Query
            var dataMashup = workbook.DataMashup;
            var formulas = dataMashup.PowerQueryFormulas;
            
            // إنشاء وإضافة صيغة جديدة (إذا لزم الأمر)
            // ملاحظة: قد يتطلب التنفيذ الفعلي نهجًا مختلفًا لإضافة الصيغ
            // لأغراض العرض، سنعمل مع الصيغ الموجودة إذا وجدت
            if (formulas.Count == 0)
            {
                // هذا فقط للعرض - قد يتطلب API الفعلي نهجًا مختلفًا
                // لإنشاء صيغ جديدة
                return;
            }

            // الوصول إلى الصيغة الأولى باستخدام خاصية Item
            var formula = formulas[0];
            
            // احصل على عناصر الصيغة
            var formulaItems = formula.PowerQueryFormulaItems;
            if (formulaItems.Count == 0)
            {
                // هذا فقط للعرض - قد يتطلب API الفعلي نهجًا مختلفًا
                // لإنشاء عناصر صيغة جديدة
                return;
            }

            // الوصول إلى العنصر الأول باستخدام خاصية Item
            var formulaItem = formulaItems[0];
            
            // تعيين والحصول على القيمة باستخدام خاصية Item
            string formulaText = "Sql.Database(\"SERVER\", \"DB\", [Query=\"SELECT * FROM TABLE\"])";
            formulaItem.Value = formulaText;
            
            // عرض استخدام خاصية Item
            string retrievedValue = formulaItems[0].Value;
            Console.WriteLine("Power Query Formula Item Value: " + retrievedValue);
            
            // احفظ المصنف
            workbook.Save("PowerQueryDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PowerQueryFormula](../../powerqueryformula/)
* class [PowerQueryFormulaCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)

---

## PowerQueryFormulaCollection indexer (2 of 2)

يحصل على [`PowerQueryFormula`](../../powerqueryformula/) حسب اسم صيغة Power Query.

```csharp
public PowerQueryFormula this[string name] { get; }
```

| معامل | الوصف |
| --- | --- |
| name | اسم العنصر. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // إنشاء مصنف بتحميل ملف موجود يحتوي على صيغ Power Query
            Workbook workbook = new Workbook("example.xlsx");
            
            // احصل على مجموعة صيغ Power Query
            PowerQueryFormulaCollection formulas = workbook.DataMashup.PowerQueryFormulas;
            
            // عرض استخدام خاصية Item
            try
            {
                // حاول الوصول إلى صيغة موجودة (إن وجدت)
                if (formulas.Count > 0)
                {
                    PowerQueryFormula formula = formulas[formulas[0].Name];
                    Console.WriteLine("First formula found: " + formula.Name);
                    Console.WriteLine("Formula definition: " + formula.FormulaDefinition);
                    Console.WriteLine("Formula type: " + formula.Type);
                }
                
                // سيؤدي هذا إلى إلقاء استثناء لصيغة غير موجودة
                PowerQueryFormula nonExistent = formulas["NonExistentFormula"];
            }
            catch (Exception ex)
            {
                Console.WriteLine("Expected error accessing non-existent formula: " + ex.Message);
            }
        }
    }
}
```

### انظر أيضًا

* class [PowerQueryFormula](../../powerqueryformula/)
* class [PowerQueryFormulaCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


