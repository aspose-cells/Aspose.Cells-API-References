---
title: "Workbook.GetDigitalSignature"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. يحصل على التوقيع الرقمي من الملف"
type: docs
url: /ar/net/aspose.cells/workbook/getdigitalsignature/
---
## Workbook.GetDigitalSignature method

يحصل على التوقيع الرقمي من الملف.

```csharp
public DigitalSignatureCollection GetDigitalSignature()
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DigitalSignatures;
    using System;

    public class WorkbookMethodGetDigitalSignatureDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات للسياق
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // استدعاء طريقة GetDigitalSignature لاسترجاع التوقيعات الرقمية
                DigitalSignatureCollection digitalSignatures = workbook.GetDigitalSignature();

                // عرض معلومات حول التوقيعات الرقمية
                if (digitalSignatures != null)
                {
                    int count = 0;
                    foreach (var signature in digitalSignatures)
                    {
                        count++;
                    }
                    Console.WriteLine("Number of digital signatures: " + count);
                    Console.WriteLine("GetDigitalSignature method called successfully");
                }
                else
                {
                    Console.WriteLine("No digital signatures found");
                }

                // احفظ المصنف
                workbook.Save("GetDigitalSignatureDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error calling GetDigitalSignature: " + ex.Message);
            }
        }
    }
}
```

### انظر أيضًا

* class [DigitalSignatureCollection](../../../aspose.cells.digitalsignatures/digitalsignaturecollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


