---
title: Cell.GetStringValue
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Gets the string value by specific formatted strategy
type: docs
url: /net/aspose.cells/cell/getstringvalue/
---
## Cell.GetStringValue method

Gets the string value by specific formatted strategy.

```csharp
public string GetStringValue(CellValueFormatStrategy formatStrategy)
```

| Parameter | Type | Description |
| --- | --- | --- |
| formatStrategy | CellValueFormatStrategy | The formatted strategy. |

### Examples

```csharp
// Called: string valueDisplayStyle = worksheet.Cells[&amp;quot;A2&amp;quot;].GetStringValue(CellValueFormatStrategy.DisplayStyle);
public static void Method_CellValueFormatStrategy_()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data to the worksheet
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Date&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(DateTime.Now);
            worksheet.Cells[&quot;B1&quot;].PutValue(&quot;Number&quot;);
            worksheet.Cells[&quot;B2&quot;].PutValue(12345.6789);
            worksheet.Cells[&quot;C1&quot;].PutValue(&quot;Text&quot;);
            worksheet.Cells[&quot;C2&quot;].PutValue(&quot;Hello World&quot;);

            // Apply different CellValueFormatStrategy to demonstrate their effects
            // None: Not formatted
            string valueNone = worksheet.Cells[&quot;A2&quot;].GetStringValue(CellValueFormatStrategy.None);
            Console.WriteLine($&quot;None: {valueNone}&quot;);

            // CellStyle: Only formatted with the cell&apos;s original style
            string valueCellStyle = worksheet.Cells[&quot;A2&quot;].GetStringValue(CellValueFormatStrategy.CellStyle);
            Console.WriteLine($&quot;CellStyle: {valueCellStyle}&quot;);

            // DisplayStyle: Formatted with the cell&apos;s displayed style
            string valueDisplayStyle = worksheet.Cells[&quot;A2&quot;].GetStringValue(CellValueFormatStrategy.DisplayStyle);
            Console.WriteLine($&quot;DisplayStyle: {valueDisplayStyle}&quot;);

            // DisplayString: Gets the displayed string shown in MS Excel
            string valueDisplayString = worksheet.Cells[&quot;A2&quot;].GetStringValue(CellValueFormatStrategy.DisplayString);
            Console.WriteLine($&quot;DisplayString: {valueDisplayString}&quot;);

            // Save the workbook to a file
            workbook.Save(&quot;CellValueFormatStrategyExample.xlsx&quot;);
            workbook.Save(&quot;CellValueFormatStrategyExample.pdf&quot;);
        }
```

### See Also

* enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


