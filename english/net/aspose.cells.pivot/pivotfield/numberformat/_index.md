---
title: PivotField.NumberFormat
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Represents the custom display format of numbers and dates
type: docs
url: /net/aspose.cells.pivot/pivotfield/numberformat/
---
## PivotField.NumberFormat property

Represents the custom display format of numbers and dates.

```csharp
public string NumberFormat { get; set; }
```

### Examples

```csharp
// Called: pTable.DataFields[0].NumberFormat = &amp;quot;$0.00&amp;quot;;
[Test]
        public void Property_NumberFormat()
        {
            Workbook workbook = new Workbook(Constants.openPivottablePath + &quot;Bad.xlsx&quot;);

            Worksheet pivotSheet = workbook.Worksheets.Add(&quot;PivotData&quot;);
            pivotSheet.Name = &quot;Summarize&quot;;

            PivotTableCollection pivotTables = pivotSheet.PivotTables;
            string source = String.Format(&quot;=&apos;Source Data&apos;!A1:D5&quot;);
            int index = pivotTables.Add(source, &quot;A1&quot;, &quot;PivotTable&quot;);
            PivotTable pTable = pivotTables[index];

            pTable.IsAutoFormat = true;
            pTable.AutoFormatType = PivotTableAutoFormatType.Classic;

            pTable.AddFieldToArea(PivotFieldType.Row, 0);
            pTable.AddFieldToArea(PivotFieldType.Row, 1);

            pTable.AddFieldToArea(PivotFieldType.Data, &quot;Sales&quot;);
            pTable.DataFields[0].Function = ConsolidationFunction.Sum;
            pTable.DataFields[0].NumberFormat = &quot;$0.00&quot;;

            if (pTable.DataField != null)
            {
                pTable.AddFieldToArea(PivotFieldType.Column, pTable.DataField);
            }

            workbook.Save(Constants.savePivottablePath + &quot;t.xlsx&quot;);
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


