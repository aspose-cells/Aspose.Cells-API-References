---
title: "PivotPageFields.PageFieldCount"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotPageFields‑egenskap. Hämtar antalet sidfält"
type: docs
url: /sv/net/aspose.cells.pivot/pivotpagefields/pagefieldcount/
---
## PivotPageFields.PageFieldCount property

Hämtar antalet sidfält.

```csharp
public int PageFieldCount { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotPageFieldsPropertyPageFieldCountDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Skapa exempelarbetsblad med data
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Name = "Data1";
            FillSampleData(sheet1);

            Worksheet sheet2 = workbook.Worksheets.Add("Data2");
            FillSampleData(sheet2);

            // Skapa ett pivotsblad
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotSheet");

            // Skapa PivotPageFields‑instans
            PivotPageFields pageFields = new PivotPageFields();

            // Lägg till sidfält för att demonstrera egenskapen PageFieldCount
            pageFields.AddPageField(new string[] { "Category1", "Category2" });
            pageFields.AddPageField(new string[] { "Region1", "Region2" });

            try
            {
                // Visa värdet för egenskapen PageFieldCount
                Console.WriteLine("Number of page fields: " + pageFields.PageFieldCount);

                // Lägg till identifiering för sidfälten
                pageFields.AddIdentify(0, new int[] { 0, 1 });
                pageFields.AddIdentify(1, new int[] { 1, 0 });

                // Verifiera att räknaren förblir densamma efter att identifieringar har lagts till
                Console.WriteLine("PageFieldCount after adding identifications: " + pageFields.PageFieldCount);

                // Skapa en pivottabell med hjälp av sidfälten
                string[] sources = { "=Data1!A1:C4", "=Data2!A1:C4" };
                pivotSheet.PivotTables.Add(sources, false, pageFields, "E3", "DemoPivot");

                // Spara arbetsboken
                workbook.Save("PageFieldCountDemo.xlsx");
                Console.WriteLine("Demo completed successfully. File saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        private static void FillSampleData(Worksheet sheet)
        {
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Category");
            cells["B1"].PutValue("Region");
            cells["C1"].PutValue("Value");

            cells["A2"].PutValue("Category1");
            cells["B2"].PutValue("Region1");
            cells["C2"].PutValue(100);

            cells["A3"].PutValue("Category2");
            cells["B3"].PutValue("Region2");
            cells["C3"].PutValue(200);
        }
    }
}
```

### Se även

* class [PivotPageFields](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


