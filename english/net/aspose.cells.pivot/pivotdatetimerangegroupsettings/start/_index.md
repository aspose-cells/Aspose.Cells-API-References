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
// Called: Console.WriteLine(string.Format("Start: {0}", columnRange.Start));//"Start: {columnRange?.Start}");
private static void Property_Start(string header, PivotTable pivotTable)
        {
            PivotDateTimeRangeGroupSettings columnRange =(PivotDateTimeRangeGroupSettings) pivotTable.ColumnFields[0].GroupSettings;

            Console.WriteLine(@"=============== {header} ================");
            if (columnRange != null)
            {

                Console.WriteLine(string.Format("Start: {0}", columnRange.Start));//"Start: {columnRange?.Start}");
                Console.WriteLine(string.Format("End: {0}", columnRange.End));//@"End: {columnRange?.End}");
                Console.WriteLine(string.Format("By: {0}", columnRange.Interval));//@"By: {columnRange?.By}");
                Console.WriteLine(string.Format("Types:{0}", String.Join(", ", columnRange.GroupByTypes)));//"Types: {String.Join(", ", columnRange?.GroupByTypes)}");
            }
            Console.WriteLine(@"=============== {header} DONE ===========");

        }
```

### See Also

* class [PivotDateTimeRangeGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


