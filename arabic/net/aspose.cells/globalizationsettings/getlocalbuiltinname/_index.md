---
title: "GlobalizationSettings.GetLocalBuiltInName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GlobalizationSettings. تحصل على النص المعتمد على اللغة للاسم المدمج وفقًا للنص القياسي المعطى"
type: docs
url: /ar/net/aspose.cells/globalizationsettings/getlocalbuiltinname/
---
## GlobalizationSettings.GetLocalBuiltInName method

يحصل على النص المعتمد على اللغة للاسم المدمج وفقًا للنص المعياري المعطى.

```csharp
public virtual string GetLocalBuiltInName(string standardName)
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

    public class GlobalizationSettingsMethodGetLocalBuiltInNameWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                string standardName = "Total";
                string localizedName = ((CustomGlobalizationSettings)workbook.Settings.GlobalizationSettings).GetLocalBuiltInName(standardName);

                Console.WriteLine($"Standard Name: {standardName}");
                Console.WriteLine($"Localized Name: {localizedName}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetLocalBuiltInName method: {ex.Message}");
            }

            workbook.Save("LocalizedBuiltInNameDemo.xlsx");
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetLocalBuiltInName(string standardName)
        {
            switch (standardName)
            {
                case "Total":
                    return "LocalizedTotal";
                case "Average":
                    return "LocalizedAverage";
                default:
                    return base.GetLocalBuiltInName(standardName);
            }
        }
    }
}
```

### انظر أيضًا

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


