---
title: PivotField.Function
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Represents the function used to summarize the PivotTable data field
type: docs
url: /net/aspose.cells.pivot/pivotfield/function/
---
## PivotField.Function property

Represents the function used to summarize the PivotTable data field.

```csharp
public ConsolidationFunction Function { get; set; }
```

### Examples

```csharp
// Called: pTable.DataFields[0].Function = ConsolidationFunction.Sum;
[Test]
        public void Property_Function()
        {
            Workbook workbook = new Workbook(Constants.openPivottablePath + "Bad.xlsx");

            Worksheet pivotSheet = workbook.Worksheets.Add("PivotData");
            pivotSheet.Name = "Summarize";

            PivotTableCollection pivotTables = pivotSheet.PivotTables;
            string source = String.Format("='Source Data'!A1:D5");
            int index = pivotTables.Add(source, "A1", "PivotTable");
            PivotTable pTable = pivotTables[index];

            pTable.IsAutoFormat = true;
            pTable.AutoFormatType = PivotTableAutoFormatType.Classic;

            pTable.AddFieldToArea(PivotFieldType.Row, 0);
            pTable.AddFieldToArea(PivotFieldType.Row, 1);

            pTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pTable.DataFields[0].Function = ConsolidationFunction.Sum;
            pTable.DataFields[0].NumberFormat = "$0.00";

            if (pTable.DataField != null)
            {
                pTable.AddFieldToArea(PivotFieldType.Column, pTable.DataField);
            }

            workbook.Save(Constants.savePivottablePath + "t.xlsx");
        }
```

### See Also

* enum [ConsolidationFunction](../../../aspose.cells/consolidationfunction/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


