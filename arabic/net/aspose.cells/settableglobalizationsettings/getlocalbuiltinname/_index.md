---
title: "SettableGlobalizationSettings.GetLocalBuiltInName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettableGlobalizationSettings. تحصل على النص المعتمد على الإعداد المحلي لاسم مدمج وفقًا للنص المعياري المعطى"
type: docs
url: /ar/net/aspose.cells/settableglobalizationsettings/getlocalbuiltinname/
---
## SettableGlobalizationSettings.GetLocalBuiltInName method

يحصل على النص المعتمد على اللغة للاسم المدمج وفقًا للنص المعياري المعطى.

```csharp
public override string GetLocalBuiltInName(string standardName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| standardName | String | نص الاسم المدمج القياسي (إعداد إقليمي en-US). |

### قيمة الإرجاع

نص معتمد على الإعداد المحلي. تم تحديد الإعداد المحلي بواسطة المصنف الذي تُستخدم له هذه الإعدادات.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetLocalBuiltInNameWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نسخة من SettableGlobalizationSettings
            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

            try
            {
                // استدعِ طريقة GetLocalBuiltInName مع اسم مدمج قياسي
                string standardName = "SUM";
                string localName = globalizationSettings.GetLocalBuiltInName(standardName);

                // اعرض النتيجة
                Console.WriteLine($"Standard name: {standardName}, Local name: {localName}");

                // تعيين اسم محلي مخصص للاسم المدمج القياسي
                globalizationSettings.SetLocalBuiltInName(standardName, "CustomSum", true);

                // احصل على الاسم المحلي مرة أخرى بعد تعيينه
                localName = globalizationSettings.GetLocalBuiltInName(standardName);
                Console.WriteLine($"After setting - Standard name: {standardName}, Local name: {localName}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetLocalBuiltInName method: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("MethodGetLocalBuiltInNameDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


