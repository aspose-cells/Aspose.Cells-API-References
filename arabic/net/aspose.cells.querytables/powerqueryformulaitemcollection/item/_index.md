---
title: "PowerQueryFormulaItemCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PowerQueryFormulaItemCollection. يحصل على PowerQueryFormulaItem حسب الفهرس في القائمة"
type: docs
url: /ar/net/aspose.cells.querytables/powerqueryformulaitemcollection/item/
---
## PowerQueryFormulaItemCollection indexer (1 of 2)

يحصل على [`PowerQueryFormulaItem`](../../powerqueryformulaitem/) حسب الفهرس في القائمة.

```csharp
public PowerQueryFormulaItem this[int index] { get; }
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
    public class PowerQueryFormulaItemCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد باستخدام قالب يحتوي على Power Query
            Workbook workbook = new Workbook();
            
            // الحصول على أول صيغة Power Query (بافتراض وجود واحدة)
            var powerQueryFormula = workbook.DataMashup.PowerQueryFormulas[0];
            
            // تعديل عناصر الصيغة باستخدام خاصية Item
            var formulaItems = powerQueryFormula.PowerQueryFormulaItems;
            if (formulaItems.Count > 0)
            {
                formulaItems[0].Value = "Sql.Database(\"SQL2K16\", \"EUC876REG\", [Query=\"select * from CANOTIFICATIONS\"])";
                
                // تحقق من التغيير
                Console.WriteLine(formulaItems[0].Value);
            }
            
            // احفظ المصنف
            workbook.Save("PowerQueryExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PowerQueryFormulaItem](../../powerqueryformulaitem/)
* class [PowerQueryFormulaItemCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)

---

## PowerQueryFormulaItemCollection indexer (2 of 2)

يحصل على [`PowerQueryFormulaItem`](../../powerqueryformulaitem/) حسب اسم العنصر.

```csharp
public PowerQueryFormulaItem this[string name] { get; }
```

| معامل | الوصف |
| --- | --- |
| name | اسم العنصر. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaItemCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            try
            {
                // تحميل مصنف يحتوي على صيغ Power Query.
                // استبدل المسار بملف فعلي يحتوي على Power Query إذا كان متاحًا.
                string sourcePath = "PowerQuerySample.xlsx";
                Workbook workbook = System.IO.File.Exists(sourcePath) ? new Workbook(sourcePath) : new Workbook();

                // الوصول إلى مجموعة صيغ Power Query.
                PowerQueryFormulaCollection pqFormulas = workbook.DataMashup.PowerQueryFormulas;

                if (pqFormulas.Count == 0)
                {
                    Console.WriteLine("No Power Query formulas found in the workbook.");
                    return;
                }

                // الحصول على أول صيغة Power Query.
                PowerQueryFormula formula = pqFormulas[0];

                // الوصول إلى مجموعة عناصره.
                PowerQueryFormulaItemCollection items = formula.PowerQueryFormulaItems;

                if (items.Count == 0)
                {
                    Console.WriteLine("The selected Power Query formula contains no items.");
                    return;
                }

                // استرجاع العنصر الأول للحصول على اسم عنصر صالح.
                PowerQueryFormulaItem firstItem = items[0];
                string itemName = firstItem.Name;

                // استخدام الفهرس Item(string) (للقراءة فقط) للحصول على نفس العنصر حسب الاسم.
                PowerQueryFormulaItem retrievedItem = items[itemName];

                // عرض خصائص العنصر المسترجع.
                Console.WriteLine($"Item Name : {retrievedItem.Name}");
                Console.WriteLine($"Item Value: {retrievedItem.Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [PowerQueryFormulaItem](../../powerqueryformulaitem/)
* class [PowerQueryFormulaItemCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


