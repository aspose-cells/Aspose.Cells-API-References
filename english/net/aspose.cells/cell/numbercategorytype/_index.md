---
title: Cell.NumberCategoryType
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Represents the category type of this cells number formatting
type: docs
url: /net/aspose.cells/cell/numbercategorytype/
---
## Cell.NumberCategoryType property

Represents the category type of this cell's number formatting.

```csharp
public NumberCategoryType NumberCategoryType { get; }
```

### Remarks

When cell's formatting pattern is combined with conditional formatting patterns, then the returned type is corresponding to the part which is used for current value of this cell. For example, if the formatting pattern for this cell is "#,##0;(#,##0);"-";@", then when cell's value is numeric and not 0, the returned type is Number; When cell's value is 0 or not numeric value, the returned type is Text.

### Examples

```csharp
// Called: Console.WriteLine(&amp;quot;Cell A1 Number Category Type: &amp;quot; + worksheet.Cells[&amp;quot;A1&amp;quot;].NumberCategoryType);
public static void Property_NumberCategoryType()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;General&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;Text&quot;);
            worksheet.Cells[&quot;A3&quot;].PutValue(12345);
            worksheet.Cells[&quot;A4&quot;].PutValue(DateTime.Now);
            worksheet.Cells[&quot;A5&quot;].PutValue(TimeSpan.FromHours(1.5));
            worksheet.Cells[&quot;A6&quot;].PutValue(0.75);
            worksheet.Cells[&quot;A7&quot;].PutValue(1.23E+3);

            // Set number formats for the cells
            worksheet.Cells[&quot;A1&quot;].SetStyle(CreateStyle(workbook, NumberCategoryType.General));
            worksheet.Cells[&quot;A2&quot;].SetStyle(CreateStyle(workbook, NumberCategoryType.Text));
            worksheet.Cells[&quot;A3&quot;].SetStyle(CreateStyle(workbook, NumberCategoryType.Number));
            worksheet.Cells[&quot;A4&quot;].SetStyle(CreateStyle(workbook, NumberCategoryType.Date));
            worksheet.Cells[&quot;A5&quot;].SetStyle(CreateStyle(workbook, NumberCategoryType.Time));
            worksheet.Cells[&quot;A6&quot;].SetStyle(CreateStyle(workbook, NumberCategoryType.Fraction));
            worksheet.Cells[&quot;A7&quot;].SetStyle(CreateStyle(workbook, NumberCategoryType.Scientific));

            // Output the number category types
            Console.WriteLine(&quot;Cell A1 Number Category Type: &quot; + worksheet.Cells[&quot;A1&quot;].NumberCategoryType);
            Console.WriteLine(&quot;Cell A2 Number Category Type: &quot; + worksheet.Cells[&quot;A2&quot;].NumberCategoryType);
            Console.WriteLine(&quot;Cell A3 Number Category Type: &quot; + worksheet.Cells[&quot;A3&quot;].NumberCategoryType);
            Console.WriteLine(&quot;Cell A4 Number Category Type: &quot; + worksheet.Cells[&quot;A4&quot;].NumberCategoryType);
            Console.WriteLine(&quot;Cell A5 Number Category Type: &quot; + worksheet.Cells[&quot;A5&quot;].NumberCategoryType);
            Console.WriteLine(&quot;Cell A6 Number Category Type: &quot; + worksheet.Cells[&quot;A6&quot;].NumberCategoryType);
            Console.WriteLine(&quot;Cell A7 Number Category Type: &quot; + worksheet.Cells[&quot;A7&quot;].NumberCategoryType);

            // Save the workbook
            workbook.Save(&quot;NumberCategoryTypeExample.xlsx&quot;);
        }
```

### See Also

* enum [NumberCategoryType](../../numbercategorytype/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


