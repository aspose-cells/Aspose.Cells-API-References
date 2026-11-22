---
title: "Workbook.UpdateLinkedDataSource"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. إذا كان هذا المصنف يحتوي على روابط خارجية إلى مصدر بيانات آخر، سيحاول Aspose.Cells استرجاع أحدث البيانات من المصادر المعطاة"
type: docs
url: /ar/net/aspose.cells/workbook/updatelinkeddatasource/
---
## Workbook.UpdateLinkedDataSource method

إذا كان هذا المصنف يحتوي على روابط خارجية إلى مصدر بيانات آخر، سيحاول Aspose.Cells استرجاع أحدث البيانات من المصادر المعطاة.

```csharp
public void UpdateLinkedDataSource(Workbook[] externalWorkbooks)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| externalWorkbooks | Workbook[] | المصنفات التي ستُستخدم لتحديث بيانات الروابط الخارجية المشار إليها من قبل هذا المصنف. يتم تحديد مطابقة تلك المصنفات مع الروابط الخارجية بواسطة [`FileName`](../filename/) و [`DataSource`](../../externallink/datasource/). لذا يرجى التأكد من أن [`FileName`](../filename/) تم تحديده بالقيمة المناسبة لكل مصنف حتى يمكن ربطه بالرابط الخارجي المقابل. |

### ملاحظات

إذا لم يتم العثور على الرابط الخارجي المقابل لمصنف واحد، فسيتم تجاهل هذا المصنف. لذا عندما تقوم بتعيين صيغة لاحقًا باستخدام رابط خارجي جديد تريد ربط المصنف المتجاهل به، لا يمكن تنفيذ الرابط حتى تستدعي هذه الطريقة مرة أخرى مع تلك المصنفات.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookMethodUpdateLinkedDataSourceWithWorkbookDemo
    {
        public static void Run()
        {
            // إنشاء مصنف رئيسي مع مراجع خارجية
            Workbook mainWorkbook = new Workbook();
            Worksheet mainSheet = mainWorkbook.Worksheets[0];
            mainSheet.Cells["A1"].Formula = "=[ExternalWorkbook.xlsx]Sheet1!A1";

            // إنشاء مصنف خارجي سيتم ربطه
            Workbook externalWorkbook = new Workbook();
            Worksheet externalSheet = externalWorkbook.Worksheets[0];
            externalSheet.Cells["A1"].Value = "Updated External Value";

            try
            {
                // استدعِ UpdateLinkedDataSource مع مصفوفة المصنفات الخارجية
                mainWorkbook.UpdateLinkedDataSource(new Workbook[] { externalWorkbook });

                // احسب الصيغ لتحديث المرجع
                mainWorkbook.CalculateFormula();

                // عرض القيمة المحدثة
                Console.WriteLine("Updated value in main workbook: " + mainSheet.Cells["A1"].Value);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UpdateLinkedDataSource method: {ex.Message}");
            }

            // حفظ النتيجة
            mainWorkbook.Save("UpdateLinkedDataSourceDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


