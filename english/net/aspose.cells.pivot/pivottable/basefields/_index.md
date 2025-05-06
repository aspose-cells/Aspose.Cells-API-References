---
title: PivotTable.BaseFields
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Returns all base pivot fields in the PivotTable
type: docs
url: /net/aspose.cells.pivot/pivottable/basefields/
---
## PivotTable.BaseFields property

Returns all base pivot fields in the PivotTable.

```csharp
public PivotFieldCollection BaseFields { get; }
```

### Examples

```csharp
// Called: pivotTable.AddFieldToArea(PivotFieldType.Data, pivotTable.BaseFields[dataField[i]]);
[Test]
        public void Property_BaseFields()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;JAVA42587_&quot;;

            String file = &quot;Forecast Sets.xlsx&quot;;
            int rowCount = 201;
            int colCount = 17;
            String pivotName = &quot;Pivot&quot;;

            String[] pageField = {&quot;Forecast Set&quot;, &quot;Created By&quot;, &quot;Creation Date&quot;, &quot;Consume&quot;, &quot;Outlier Update Percentage&quot;, &quot;Backward Days&quot;, &quot;Foreward Days&quot;, &quot;Forecast&quot;,
                    &quot;Forecast Description&quot;, &quot;Demand Class&quot;, &quot;Customer Name&quot;, &quot;Bill Address&quot;, &quot;Ship Address&quot;, &quot;Disable Date&quot;, &quot;Level1&quot;};
            String[] columnField = { &quot;Bucket Type&quot; };
            String[] rowField = { &quot;Organization Code&quot; };
            String[] dataField = { };

            Workbook workbook = new Workbook(filePath + file);
            String sourceData = &quot;&apos;Data&apos;!$A$&quot; + (1) + &quot;:&quot; + CellsHelper.CellIndexToName(rowCount, colCount - 1);

            Worksheet worksheet = workbook.Worksheets.Add(pivotName);
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add(sourceData, &quot;A10&quot;, pivotName);
            PivotTable pivotTable = (PivotTable)pivotTables[index];
            pivotTable.Name = pivotName;

            pivotTable.IsGridDropZones = true;

            for (int i = 0; i &lt; columnField.Length; i++)
            {
                pivotTable.AddFieldToArea(PivotFieldType.Column, pivotTable.BaseFields[columnField[i]]);
            }

            for (int i = 0; i &lt; pageField.Length; i++)
            {
                pivotTable.AddFieldToArea(PivotFieldType.Page, pivotTable.BaseFields[pageField[i]]);
            }

            for (int i = 0; i &lt; rowField.Length; i++)
            {
                pivotTable.AddFieldToArea(PivotFieldType.Row, pivotTable.BaseFields[rowField[i]]);
            }

            pivotTable.IsAutoFormat = true;
            pivotTable.AutoFormatType = PivotTableAutoFormatType.None;
            pivotTable.PageFieldOrder = PrintOrderType.DownThenOver;
            pivotTable.PageFieldWrapCount = 5;

            for (int i = 0; i &lt; dataField.Length; i++)
            {
                pivotTable.AddFieldToArea(PivotFieldType.Data, pivotTable.BaseFields[dataField[i]]);
            }

            pivotTable.SaveData = true;
            pivotTable.PreserveFormatting = true;
            workbook.Save(CreateFolder(filePath) + &quot;out.xlsx&quot;);
        }
```

### See Also

* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


