---
title: "SettableGlobalizationSettings.SetStandardBuiltInName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettableGlobalizationSettings. تعيين اسم الدالة المعتمد على الإعدادات المحلية وفقًا لاسم الدالة القياسي المعطى"
type: docs
url: /ar/net/aspose.cells/settableglobalizationsettings/setstandardbuiltinname/
---
## SettableGlobalizationSettings.SetStandardBuiltInName method

يضبط اسم الدالة المعتمد على الإعدادات الإقليمية وفقًا لاسم الدالة القياسي المعطى.

```csharp
public void SetStandardBuiltInName(string localName, string standardName, bool bidirectional)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| localName | String | اسم الدالة المعتمد على الإعدادات المحلية |
| standardName | String | اسم الدالة القياسي (إعداد محلي en-US). |
| bidirectional | Boolean | ما إذا كان سيتم ربط نص الاسم القياسي بنص الاسم المحلي تلقائيًا. إذا كان صحيحًا، سيتم ربط نص الاسم القياسي بنص الاسم المحلي تلقائيًا بحيث لا يحتاج المستخدم إلى استدعاء [`SetLocalBuiltInName`](../setlocalbuiltinname/) مرة أخرى لنفس زوج الأسماء القياسية والمحلية. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetStandardBuiltInNameWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إنشاء إعدادات تعميم مخصصة
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // تعيين إعدادات العولمة لدفتر العمل
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // استدعِ SetStandardBuiltInName لربط اسم محلي باسم قياسي مدمج
                // المعلمات: localName، standardName، bidirectional
                settings.SetStandardBuiltInName("MyLocalName", "SUM", true);
                
                Console.WriteLine("SetStandardBuiltInName executed successfully with parameters (\"MyLocalName\", \"SUM\", true)");
                
                // أظهر التأثير باستخدام الاسم المحلي في صيغة
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["A2"].PutValue(20);
                worksheet.Cells["A3"].Formula = "=MyLocalName(A1:A2)";
                
                // احسب الصيغة لإظهار أنها تعمل بالاسم المحلي
                workbook.CalculateFormula();
                Console.WriteLine("Result of formula with local name: " + worksheet.Cells["A3"].Value);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetStandardBuiltInName method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("SetStandardBuiltInNameDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


