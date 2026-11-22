---
title: "LoadOptions.LanguageCode"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LoadOptions. تحصل أو تعين لغة واجهة المستخدم لإصدار المصنف بناءً على CountryCode الذي حفظ الملف"
type: docs
url: /ar/net/aspose.cells/loadoptions/languagecode/
---
## LoadOptions.LanguageCode property

يحصل أو يضبط لغة واجهة المستخدم لإصدار Workbook بناءً على رمز البلد (CountryCode) الذي حفظ الملف.

```csharp
public CountryCode LanguageCode { get; set; }
```

### أمثلة

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyLanguageCodeDemo
    {
        public static void Run()
        {
            // إنشاء مثال من LoadOptions
            LoadOptions loadOptions = new LoadOptions();

            // عيّن خاصية LanguageCode
            loadOptions.LanguageCode = CountryCode.USA;

            // تحميل مصنف باستخدام LoadOptions المحددة
            Workbook workbook = new Workbook("sample.xlsx", loadOptions);

            // الوصول إلى ورقة العمل وتعديل المحتوى
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Language Code Demo");

            // احفظ المصنف المعدل
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [CountryCode](../../countrycode/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


