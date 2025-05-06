---
title: PivotTable.AddCalculatedField
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Adds a calculated field to pivot field
type: docs
url: /net/aspose.cells.pivot/pivottable/addcalculatedfield/
---
## AddCalculatedField(string, string, bool) {#addcalculatedfield_1}

Adds a calculated field to pivot field.

```csharp
public void AddCalculatedField(string name, string formula, bool dragToDataArea)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the calculated field |
| formula | String | The formula of the calculated field. |
| dragToDataArea | Boolean | True,drag this field to data area immediately |

### Examples

```csharp
// Called: pt.AddCalculatedField(&amp;quot;testcalfld&amp;quot;, &amp;quot;=Sales*2&amp;quot;, true);
[Test]
        public void Method_Boolean_()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET50981_&quot;;

            Workbook wb = new Workbook(filePath + &quot;calField.xlsx&quot;);
            Worksheet sheet = wb.Worksheets[0];
            PivotTableCollection pivotTables = sheet.PivotTables;
            PivotTable pt = pivotTables[0];
            pt.AddCalculatedField(&quot;testcalfld&quot;, &quot;=Sales*2&quot;, true);

        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## AddCalculatedField(string, string) {#addcalculatedfield}

Adds a calculated field to pivot field and drag it to data area.

```csharp
public void AddCalculatedField(string name, string formula)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the calculated field |
| formula | String | The formula of the calculated field. |

### Examples

```csharp
// Called: pivotTable.AddCalculatedField(&amp;quot;Price&amp;quot;, &amp;quot;&amp;apos;Value&amp;apos; / &amp;apos;Units&amp;apos;&amp;quot;);
[Test]
        public void Method_String_()
        {
            Workbook workbook = new Workbook();

            // put in data
            Worksheet data = workbook.Worksheets.Add(&quot;data&quot;);
            data.Cells[&quot;A1&quot;].PutValue(&quot;Country&quot;);
            data.Cells[&quot;B1&quot;].PutValue(&quot;Product&quot;);
            data.Cells[&quot;C1&quot;].PutValue(&quot;Vendor&quot;);
            data.Cells[&quot;D1&quot;].PutValue(&quot;Value&quot;);
            data.Cells[&quot;E1&quot;].PutValue(&quot;Units&quot;);
            data.Cells[&quot;A2&quot;].PutValue(&quot;USA&quot;);
            data.Cells[&quot;B2&quot;].PutValue(&quot;Car&quot;);
            data.Cells[&quot;C2&quot;].PutValue(&quot;Ford&quot;);
            data.Cells[&quot;D2&quot;].PutValue(1200.987654321);
            data.Cells[&quot;E2&quot;].PutValue(3);
            data.Cells[&quot;A3&quot;].PutValue(&quot;Japan&quot;);
            data.Cells[&quot;B3&quot;].PutValue(&quot;Bike&quot;);
            data.Cells[&quot;C3&quot;].PutValue(&quot;Yamaha&quot;);
            data.Cells[&quot;D3&quot;].PutValue(985.123456789);
            data.Cells[&quot;E3&quot;].PutValue(2);

            // create pivot
            Worksheet pivot = workbook.Worksheets.Add(&quot;pivot&quot;);
            PivotTableCollection pivotTables = pivot.PivotTables;
            int index = pivotTables.Add(&quot;=data!A1:E3&quot;, &quot;A1&quot;, &quot;pivotTable1&quot;,false,true);
            PivotTable pivotTable = pivotTables[index];
            pivotTable.ShowRowGrandTotals = (false);
            pivotTable.ShowColumnGrandTotals = (true);
            pivotTable.IsGridDropZones = (true);
            pivotTable.RefreshDataOnOpeningFile = (false);
            pivotTable.AddFieldToArea(PivotFieldType.Row, &quot;Country&quot;);
            pivotTable.AddFieldToArea(PivotFieldType.Column, &quot;Product&quot;);
            pivotTable.AddFieldToArea(PivotFieldType.Page, &quot;Vendor&quot;);
            pivotTable.AddFieldToArea(PivotFieldType.Data, &quot;Value&quot;);
            pivotTable.AddFieldToArea(PivotFieldType.Data, &quot;Units&quot;);



            pivotTable.AddCalculatedField(&quot;Price&quot;, &quot;&apos;Value&apos; / &apos;Units&apos;&quot;);
            Assert.IsFalse(pivotTable.BaseFields[5].ShowCompact);
            // recalculate data in pivot according to new setup
            pivotTable.CalculateRange();
            pivotTable.CalculateData();
            pivotTable.PageFieldWrapCount = (0);
            Assert.AreEqual(&quot;Country&quot;, pivot.Cells[&quot;A4&quot;].StringValue);
            workbook.Save(Constants.PivotTableDestPath + &quot;CELLSJAVA46206.xlsx&quot;);
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


