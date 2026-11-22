---
title: "PowerQueryFormulaParameter.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PowerQueryFormulaParameter. تحصل على نوع power query formula"
type: docs
url: /ar/net/aspose.cells.querytables/powerqueryformulaparameter/type/
---
## PowerQueryFormulaParameter.Type property

يحصل على نوع صيغة استعلام الطاقة.

```csharp
public override PowerQueryFormulaType Type { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaParameterPropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            try
            {
                // نظرًا لأننا لا نستطيع إنشاء PowerQueryFormulaParameter مباشرةً دون معرفة معلمات المنشئ المطلوبة،
                // سنوضح الوصول إلى خاصية Type عبر معاملات جدول استعلام موجود
                Console.WriteLine("This demo shows how to access the Type property of PowerQueryFormulaParameter.");
                
                // في سيناريو واقعي، ستصل إلى ذلك من جدول استعلام موجود
                // لأغراض العرض، سنظهر كيفية فحص النوع إذا كان لديك مثال
                PowerQueryFormulaParameter parameter = null; // This would normally come from a query table
                
                if (parameter != null)
                {
                    // عرض قيمة خاصية Type (خاصية للقراءة فقط)
                    Console.WriteLine($"PowerQueryFormulaParameter Type: {parameter.Type}");
                    
                    // عرض القيم الممكنة للتعداد
                    Console.WriteLine("Possible PowerQueryFormulaType values:");
                    foreach (PowerQueryFormulaType type in Enum.GetValues(typeof(PowerQueryFormulaType)))
                    {
                        Console.WriteLine($"- {type}");
                    }
                }
                else
                {
                    Console.WriteLine("No PowerQueryFormulaParameter instance available for demonstration.");
                }
                
                // احفظ المصنف
                workbook.Save("TypeDemo.xlsx");
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

* enum [PowerQueryFormulaType](../../powerqueryformulatype/)
* class [PowerQueryFormulaParameter](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


