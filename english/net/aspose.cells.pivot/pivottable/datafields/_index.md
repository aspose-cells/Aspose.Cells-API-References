---
title: PivotTable.DataFields
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Gets a PivotField object that represents all the data fields in a PivotTable. Readonly.It would be init only when there are two or more data fields in the DataPiovtFiels. It only use to add DataPivotField to the PivotTable row/column area . Default is in row area
type: docs
url: /net/aspose.cells.pivot/pivottable/datafields/
---
## PivotTable.DataFields property

Gets a PivotField object that represents all the data fields in a PivotTable. Read-only.It would be init only when there are two or more data fields in the DataPiovtFiels. It only use to add DataPivotField to the PivotTable row/column area . Default is in row area.

```csharp
public PivotFieldCollection DataFields { get; }
```

### Examples

```csharp
// Called: pivot.DataFields[0].Function = ConsolidationFunction.Sum;
[Test]
        public void Property_DataFields()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET42655_&quot;;
            Workbook wb = new Workbook(filePath + &quot;pastry2_desired.xlsx&quot;);
            Worksheet pivotSheet = wb.Worksheets.Add(&quot;GroupPivotTable&quot;);

            int pivotIndex = pivotSheet.PivotTables.Add(&quot;=PastrySalesData!A1:D16&quot;, &quot;A3&quot;, &quot;groupPivot&quot;);
            PivotTable pivot = pivotSheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Page, &quot;Testing&quot;);
            pivot.AddFieldToArea(PivotFieldType.Row, &quot;Name&quot;);
            pivot.AddFieldToArea(PivotFieldType.Column, &quot;Date&quot;);
            pivot.AddFieldToArea(PivotFieldType.Data, &quot;NumberOfOrders&quot;);

            pivot.DataFields[0].Function = ConsolidationFunction.Sum;

            PivotField dateBaseField = pivot.BaseFields[&quot;Date&quot;];

            DateTime start = new DateTime(2013, 1, 1);
            DateTime end = new DateTime(2013, 12, 31);
            ArrayList groupTypeList = new ArrayList();
            groupTypeList.Add(PivotGroupByType.Months);
            groupTypeList.Add(PivotGroupByType.Years);
           // pivot.SetManualGroupField(dateBaseField, start, end, groupTypeList, 1);
              dateBaseField.GroupBy(start, end, new PivotGroupByType[] { PivotGroupByType.Months, PivotGroupByType.Years }, 1, false);
          
            pivot.RefreshData();
            pivot.CalculateData();
           
            wb.Save(CreateFolder(filePath) + &quot;out.xlsx&quot;);
            Assert.AreEqual(pivotSheet.Cells[&quot;B4&quot;].StringValue, &quot;2013&quot;);
            Assert.AreEqual(pivotSheet.Cells[&quot;B5&quot;].StringValue, &quot;Jan&quot;);
            wb.Save(CreateFolder(filePath) + &quot;out.pdf&quot;);
           
        }
```

### See Also

* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


