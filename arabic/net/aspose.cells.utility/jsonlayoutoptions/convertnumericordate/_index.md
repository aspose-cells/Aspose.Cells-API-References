---
title: "JsonLayoutOptions.ConvertNumericOrDate"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية JsonLayoutOptions. تشير إلى ما إذا كان يتم تحويل السلسلة في json إلى قيمة رقمية أو تاريخية"
type: docs
url: /ar/net/aspose.cells.utility/jsonlayoutoptions/convertnumericordate/
---
## JsonLayoutOptions.ConvertNumericOrDate property

يشير إلى ما إذا كان يتم تحويل السلسلة في json إلى قيمة رقمية أو تاريخية.

```csharp
public bool ConvertNumericOrDate { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsPropertyConvertNumericOrDateDemo
    {
        public static void Run()
        {
            string jsonData = "[{\"ID\":101,\"Name\":\"John Doe\",\"BirthDate\":\"15-05-1990\",\"Salary\":75000.50}]";

            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            JsonLayoutOptions layoutOptions = new JsonLayoutOptions();
            layoutOptions.ArrayAsTable = true;
            layoutOptions.ConvertNumericOrDate = true;
            layoutOptions.DateFormat = "dd-MM-yyyy";
            layoutOptions.NumberFormat = "#,##0.00";

            JsonUtility.ImportData(jsonData, worksheet.Cells, 0, 0, layoutOptions);

            Console.WriteLine("Cell A2 (ID) type: " + worksheet.Cells["A2"].Type); // Should be numeric
            Console.WriteLine("Cell C2 (BirthDate) type: " + worksheet.Cells["C2"].Type); // Should be DateTime
            Console.WriteLine("Cell D2 (Salary) value: " + worksheet.Cells["D2"].Value); // Should be formatted number

            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


