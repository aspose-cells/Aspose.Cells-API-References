---
title: "PivotPageFields.AddPageField"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotPageFields. تضيف حقل صفحة"
type: docs
url: /ar/net/aspose.cells.pivot/pivotpagefields/addpagefield/
---
## PivotPageFields.AddPageField method

يضيف حقل صفحة.

```csharp
public void AddPageField(string[] pageItems)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| pageItems | String[] | تسمية عنصر حقل الصفحة |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotPageFieldsMethodAddPageFieldWithStringArrayDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.Cells["A1"].PutValue("Region");
            worksheet.Cells["A2"].PutValue("North");
            worksheet.Cells["A3"].PutValue("South");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(1500);

            string[] consolidationRanges = { "A1:B3" };
            PivotPageFields pageFields = new PivotPageFields();
            int pivotIndex = worksheet.PivotTables.Add(
                consolidationRanges,
                false,
                pageFields,
                "D1",
                "MyPivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            try
            {
                pageFields.AddPageField(new string[] { "North", "South" });
                Console.WriteLine("AddPageField executed successfully with parameters (String[])");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("AddPageFieldStringArrayDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotPageFields](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


