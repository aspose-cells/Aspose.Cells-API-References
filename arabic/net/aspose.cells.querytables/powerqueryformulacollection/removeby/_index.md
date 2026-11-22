---
title: "PowerQueryFormulaCollection.RemoveBy"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PowerQueryFormulaCollection. إزالة صيغة Power Query حسب الاسم"
type: docs
url: /ar/net/aspose.cells.querytables/powerqueryformulacollection/removeby/
---
## PowerQueryFormulaCollection.RemoveBy method

إزالة صيغة Power Query بالاسم.

```csharp
public void RemoveBy(string name)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم صيغة Power Query. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaCollectionMethodRemoveByWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            try
            {
                // الوصول إلى PowerQueryFormulaCollection (على افتراض أنها موجودة في المصنف)
                PowerQueryFormulaCollection powerQueryFormulas = workbook.DataMashup.PowerQueryFormulas;
                
                // إضافة صيغة نموذجية لإزالتها (عادةً ما تكون من البيانات الموجودة)
                string formulaName = "SampleFormula";
                
                // استدعاء RemoveBy مع اسم الصيغة
                powerQueryFormulas.RemoveBy(formulaName);
                
                Console.WriteLine($"Formula '{formulaName}' removed successfully");
                
                // احفظ المصنف
                workbook.Save("RemoveByWithStringDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in RemoveBy demonstration: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [PowerQueryFormulaCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


