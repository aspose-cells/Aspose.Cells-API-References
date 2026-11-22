---
title: "Name.GetReferredAreas"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Name. يحصل على جميع المراجع المشار إليها بهذا الاسم"
type: docs
url: /ar/net/aspose.cells/name/getreferredareas/
---
## Name.GetReferredAreas method

يحصل على جميع الإشارات التي يُشير إليها هذا الاسم.

```csharp
public ReferredArea[] GetReferredAreas(bool recalculate)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| إعادة حساب | منطقي | ما إذا كان يجب إعادة حسابه إذا تم حساب هذا الاسم مسبقًا قبل هذا الاستدعاء. |

### قيمة الإرجاع

جميع النطاقات.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameMethodGetReferredAreasWithBooleanDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook wb = new Workbook();
            
            // أضف بعض البيانات إلى ورقة العمل
            wb.Worksheets[0].Cells[3, 3].PutValue("v03");
            
            // إنشاء نطاق مسمى مع مراجع متعددة
            Name n = wb.Worksheets.Names[wb.Worksheets.Names.Add("testname")];
            n.RefersTo = "='C:\\[extlink1.xlsx]Sheet1'!$A$1:$B$2,'C:\\[extlink2.xlsx]Sheet2'!$C$3,Sheet1!$D$4,'C:\\[extlink1.xlsx]Sheet1'!E5";
            
            // احصل على المناطق المشار إليها مع روابط خارجية
            ReferredArea[] ras = n.GetReferredAreas(true);
            
            // عرض المعلومات حول كل منطقة مشار إليها
            Console.WriteLine("Number of referred areas: " + ras.Length);
            for (int i = 0; i < ras.Length; i++)
            {
                ReferredArea ra = ras[i];
                Console.WriteLine($"\nArea {i + 1}:");
                Console.WriteLine($"IsExternalLink: {ra.IsExternalLink}");
                if (ra.IsExternalLink)
                {
                    Console.WriteLine($"ExternalFileName: {ra.ExternalFileName}");
                }
                Console.WriteLine($"SheetName: {ra.SheetName}");
                Console.WriteLine($"IsArea: {ra.IsArea}");
                
                if (ra.IsArea)
                {
                    Console.WriteLine($"Range: {CellsHelper.CellIndexToName(ra.StartRow, ra.StartColumn)}" +
                                    $" to {CellsHelper.CellIndexToName(ra.EndRow, ra.EndColumn)}");
                }
                else
                {
                    Console.WriteLine($"Cell: {CellsHelper.CellIndexToName(ra.StartRow, ra.StartColumn)}");
                }
            }
            
            // إنشاء دفتر عمل خارجي وتحديث القيم
            Workbook wb1 = new Workbook();
            wb1.Worksheets[0].Cells[0, 0].PutValue("v10");
            wb1.Worksheets[0].Cells[1, 1].PutValue("v11");
            wb1.Worksheets[0].Cells[4, 4].PutValue("v14");
            
            // تحديث مصدر البيانات المرتبط
            wb.UpdateLinkedDataSource(new Workbook[]{wb1});
            
            // عرض بعض القيم من المناطق المشار إليها
            Console.WriteLine("\nValues from referred areas:");
            Console.WriteLine($"Area1[0,0]: {ras[0].GetValue(0, 0)}");
            Console.WriteLine($"Area1[1,1]: {ras[0].GetValue(1, 1)}");
            Console.WriteLine($"Area3[0,0]: {ras[2].GetValue(0, 0)}");
            Console.WriteLine($"Area4[0,0]: {ras[3].GetValue(0, 0)}");
        }
    }
}
```

### انظر أيضًا

* class [ReferredArea](../../referredarea/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


