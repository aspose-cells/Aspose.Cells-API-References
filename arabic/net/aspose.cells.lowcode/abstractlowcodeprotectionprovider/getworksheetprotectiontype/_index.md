---
title: "AbstractLowCodeProtectionProvider.GetWorksheetProtectionType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة AbstractLowCodeProtectionProvider. تحصل على نوع الحماية لحماية ورقة العمل المحددة"
type: docs
url: /ar/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworksheetprotectiontype/
---
## AbstractLowCodeProtectionProvider.GetWorksheetProtectionType method

يحصل على نوع الحماية لحماية ورقة العمل المحددة.

```csharp
public virtual ProtectionType GetWorksheetProtectionType(string sheetName)
```

### قيمة الإرجاع

نوع الحماية لحماية ورقة العمل المحددة. لا شيء يعني عدم وجود حماية لورقة العمل.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeProtectionProviderMethodGetWorksheetProtectionTypeWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets.Add("newSheet");
            string name = worksheet.Name;
            var protectionProvider = new CustomProtectionProvider();

            try
            {
                worksheet.Protect(protectionProvider.GetWorksheetProtectionType(name), protectionProvider.GetWorksheetPassword(name), "");
               
                // اعرض النتيجة
                Console.WriteLine($"Worksheet '{name}' protection type: {protectionProvider.GetWorksheetProtectionType(name)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error retrieving protection type: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("GetWorksheetProtectionTypeDemo.xlsx");
        }

        private class CustomProtectionProvider : AbstractLowCodeProtectionProvider
        {
            public override ProtectionType GetWorksheetProtectionType(string sheetName)
            {
                return ProtectionType.Structure;
            }

            public override string GetWorksheetPassword(string sheetName)
            {
                return $"aspose123_{sheetName}";
            }
        }

    }
    
}
```

### انظر أيضًا

* enum [ProtectionType](../../../aspose.cells/protectiontype/)
* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


