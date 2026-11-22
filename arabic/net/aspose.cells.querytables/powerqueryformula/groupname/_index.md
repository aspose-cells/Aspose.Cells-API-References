---
title: "PowerQueryFormula.GroupName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PowerQueryFormula. يحصل على اسم المجموعة التي تحتوي على هذه صيغة Power Query"
type: docs
url: /ar/net/aspose.cells.querytables/powerqueryformula/groupname/
---
## PowerQueryFormula.GroupName property

يحصل على اسم المجموعة التي تحتوي على صيغة استعلام Power Query هذه.

```csharp
public string GroupName { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaPropertyGroupNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة صيغة Power Query (محاكاة لأننا لا نستطيع إنشاء PowerQueryFormulas فعلية مباشرةً)
            // عادةً ما ستقوم بتحميل ملف موجود يحتوي على صيغ Power Query
            string sourcePath = "example.xlsx";
            
            try
            {
                workbook = new Workbook(sourcePath);
                PowerQueryFormulaCollection queries = workbook.DataMashup.PowerQueryFormulas;
                
                if (queries.Count > 0)
                {
                    Console.WriteLine("First Power Query Formula Group Name: " + queries[0].GroupName);
                    
                    // توضيح الوصول إلى خاصية GroupName
                    string groupName = queries[0].GroupName;
                    Console.WriteLine($"Group Name: {groupName}");
                    
                    // احفظ وأعد التحميل لإظهار الاستمرارية
                    string destPath = "output.xlsx";
                    workbook.Save(destPath);
                    
                    Workbook workbook2 = new Workbook(destPath);
                    PowerQueryFormulaCollection queries2 = workbook2.DataMashup.PowerQueryFormulas;
                    if (queries2.Count > 0)
                    {
                        Console.WriteLine("After reload - Group Name: " + queries2[0].GroupName);
                    }
                }
                else
                {
                    Console.WriteLine("No Power Query formulas found in the file.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
                Console.WriteLine("Please ensure the example.xlsx file exists and contains Power Query formulas.");
            }
        }
    }
}
```

### انظر أيضًا

* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


