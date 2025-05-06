---
title: PivotGlobalizationSettings.GetTextOfDataFieldHeader
second_title: Aspose.Cells for .NET API Reference
description: PivotGlobalizationSettings method. Gets the the text of the value area field header in the PivotTable
type: docs
url: /net/aspose.cells.settings/pivotglobalizationsettings/gettextofdatafieldheader/
---
## PivotGlobalizationSettings.GetTextOfDataFieldHeader method

Gets the the text of the value area field header in the PivotTable.

```csharp
public virtual string GetTextOfDataFieldHeader()
```

### Return Value

The text of data field header name

### Examples

```csharp
// Called: Console.WriteLine(&amp;quot;Text of Data Field Header: &amp;quot; + globalizationSettings.GetTextOfDataFieldHeader());
public static void Method_GetTextOfDataFieldHeader()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Category&quot;);
            worksheet.Cells[&quot;B1&quot;].PutValue(&quot;Amount&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;Fruit&quot;);
            worksheet.Cells[&quot;B2&quot;].PutValue(100);
            worksheet.Cells[&quot;A3&quot;].PutValue(&quot;Vegetable&quot;);
            worksheet.Cells[&quot;B3&quot;].PutValue(200);
            worksheet.Cells[&quot;A4&quot;].PutValue(&quot;Fruit&quot;);
            worksheet.Cells[&quot;B4&quot;].PutValue(150);
            worksheet.Cells[&quot;A5&quot;].PutValue(&quot;Vegetable&quot;);
            worksheet.Cells[&quot;B5&quot;].PutValue(250);

            // Create a pivot table
            int pivotIndex = worksheet.PivotTables.Add(&quot;A1:B5&quot;, &quot;D1&quot;, &quot;PivotTable1&quot;);
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Add fields to the pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Create an instance of PivotGlobalizationSettings
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

            // Demonstrate the use of various methods
            Console.WriteLine(&quot;Text of Total: &quot; + globalizationSettings.GetTextOfTotal());
            Console.WriteLine(&quot;Text of Grand Total: &quot; + globalizationSettings.GetTextOfGrandTotal());
            Console.WriteLine(&quot;Text of Multiple Items: &quot; + globalizationSettings.GetTextOfMultipleItems());
            Console.WriteLine(&quot;Text of All: &quot; + globalizationSettings.GetTextOfAll());
            Console.WriteLine(&quot;Text of Protection: &quot; + globalizationSettings.GetTextOfProtection());
            Console.WriteLine(&quot;Text of Column Labels: &quot; + globalizationSettings.GetTextOfColumnLabels());
            Console.WriteLine(&quot;Text of Row Labels: &quot; + globalizationSettings.GetTextOfRowLabels());
            Console.WriteLine(&quot;Text of Empty Data: &quot; + globalizationSettings.GetTextOfEmptyData());
            Console.WriteLine(&quot;Text of Data Field Header: &quot; + globalizationSettings.GetTextOfDataFieldHeader());
            Console.WriteLine(&quot;Text of Years: &quot; + globalizationSettings.GetTextOfYears());
            Console.WriteLine(&quot;Text of Quarters: &quot; + globalizationSettings.GetTextOfQuarters());
            Console.WriteLine(&quot;Text of Months: &quot; + globalizationSettings.GetTextOfMonths());
            Console.WriteLine(&quot;Text of Days: &quot; + globalizationSettings.GetTextOfDays());
            Console.WriteLine(&quot;Text of Hours: &quot; + globalizationSettings.GetTextOfHours());
            Console.WriteLine(&quot;Text of Minutes: &quot; + globalizationSettings.GetTextOfMinutes());
            Console.WriteLine(&quot;Text of Seconds: &quot; + globalizationSettings.GetTextOfSeconds());
            Console.WriteLine(&quot;Text of Range: &quot; + globalizationSettings.GetTextOfRange());

            // Example of GetTextOfProtectedName method
            string protectedName = &quot;ProtectedNameExample&quot;;
            Console.WriteLine(&quot;Text of Protected Name: &quot; + globalizationSettings.GetTextOfProtectedName(protectedName));

            // Example of GetTextOfSubTotal method
            PivotFieldSubtotalType subTotalType = PivotFieldSubtotalType.Sum;
            Console.WriteLine(&quot;Text of SubTotal (Sum): &quot; + globalizationSettings.GetTextOfSubTotal(subTotalType));

            // Save the workbook
            workbook.Save(&quot;PivotGlobalizationSettingsExample.xlsx&quot;);
        }
```

### See Also

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


