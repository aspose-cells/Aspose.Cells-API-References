---
title: PivotDateTimeRangeGroupSettings.Start
second_title: Aspose.Cells for .NET API Reference
description: PivotDateTimeRangeGroupSettings property. Gets the start date time of the group
type: docs
url: /net/aspose.cells.pivot/pivotdatetimerangegroupsettings/start/
---
## PivotDateTimeRangeGroupSettings.Start property

Gets the start date time of the group.

```csharp
public DateTime Start { get; }
```

### Examples

```csharp
// Called: Console.WriteLine(string.Format(&amp;quot;Start: {0}&amp;quot;, columnRange.Start));//&amp;quot;Start: {columnRange?.Start}&amp;quot;);
private static void Property_Start(string header, PivotTable pivotTable)
        {
            PivotDateTimeRangeGroupSettings columnRange =(PivotDateTimeRangeGroupSettings) pivotTable.ColumnFields[0].GroupSettings;

            Console.WriteLine(@&quot;=============== {header} ================&quot;);
            if (columnRange != null)
            {

                Console.WriteLine(string.Format(&quot;Start: {0}&quot;, columnRange.Start));//&quot;Start: {columnRange?.Start}&quot;);
                Console.WriteLine(string.Format(&quot;End: {0}&quot;, columnRange.End));//@&quot;End: {columnRange?.End}&quot;);
                Console.WriteLine(string.Format(&quot;By: {0}&quot;, columnRange.Interval));//@&quot;By: {columnRange?.By}&quot;);
                Console.WriteLine(string.Format(&quot;Types:{0}&quot;, String.Join(&quot;, &quot;, columnRange.GroupByTypes)));//&quot;Types: {String.Join(&quot;, &quot;, columnRange?.GroupByTypes)}&quot;);
            }
            Console.WriteLine(@&quot;=============== {header} DONE ===========&quot;);

        }
```

### See Also

* class [PivotDateTimeRangeGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


