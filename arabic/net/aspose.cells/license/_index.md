---
title: "الفئة License"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.License. توفر طرقًا لترخيص المكوّن."
type: docs
url: /ar/net/aspose.cells/license/
---
## License class

يوفر طرقًا لترخيص المكوّن.

```csharp
public class License
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [License](license/)() | يُنشئ مثيلًا جديدًا لهذه الفئة. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [SetLicense](../../aspose.cells/license/setlicense/#setlicense)(Stream) | يرخص المكوّن. |
| [SetLicense](../../aspose.cells/license/setlicense/#setlicense_1)(string) | يرخص المكوّن. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LicenseDemo
    {
        public static void LicenseExample()
        {
            // إنشاء كائن من الفئة License
            License license = new License();

            // تعيين الترخيص باستخدام اسم ملف الترخيص
            license.SetLicense("Aspose.Cells.NET.lic");

            // بدلاً من ذلك، تعيين الترخيص باستخدام تدفق
            using (FileStream licenseStream = new FileStream("Aspose.Cells.NET.lic", FileMode.Open))
            {
                license.SetLicense(licenseStream);
            }

            // كود إضافي لتوضيح استخدام وظائف Aspose.Cells المرخصة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue("Hello, Aspose.Cells!");

            // احفظ المصنف للتحقق من تطبيق الترخيص بشكل صحيح
            workbook.Save("LicensedWorkbook.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


