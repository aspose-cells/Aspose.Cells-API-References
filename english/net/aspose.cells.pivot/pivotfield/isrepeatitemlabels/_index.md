---
title: PivotField.IsRepeatItemLabels
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Indicates whether repeating labels of the field in the region. The default value is false
type: docs
url: /net/aspose.cells.pivot/pivotfield/isrepeatitemlabels/
---
## PivotField.IsRepeatItemLabels property

Indicates whether repeating labels of the field in the region. The default value is false.

```csharp
public bool IsRepeatItemLabels { get; set; }
```

### Examples

```csharp
// Called: field.IsRepeatItemLabels = true;
[Test]
        public void Property_IsRepeatItemLabels()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;JAVA41551_&quot;;
            Workbook wb = new Workbook(filePath + &quot;Bk_itemsrepeattest1.xlsx&quot;);
            //Get the pivot table
            PivotTable p = wb.Worksheets[1].PivotTables[0];
            //get row PivotField collection
            PivotFieldCollection rowsF = p.RowFields;
            //get PivotField named &quot;Netting ID&quot;
            PivotField f = rowsF[&quot;Netting ID&quot;];

            //set RepeatItemLabels is true
            f.IsRepeatItemLabels = true;

            p.RefreshData();
            p.CalculateData();
            p.RefreshDataOnOpeningFile = false;

            Cells cells = wb.Worksheets[1].Cells;
            Assert.AreEqual(cells[&quot;B11&quot;].StringValue, &quot;(blank)&quot;);
            Assert.AreEqual(cells[&quot;B12&quot;].StringValue, &quot;(blank)&quot;);

            Assert.AreEqual(cells[&quot;B91&quot;].StringValue, &quot;1&quot;);
            Assert.AreEqual(cells[&quot;B92&quot;].StringValue, &quot;1&quot;);
            wb.Save(Constants.PivotTableDestPath + @&quot;JAVA41551Bk_itemsrepeattest1_out.xlsx&quot;);


            Workbook workbook = new Workbook(filePath + &quot;eld81213_Copy+of+BOM+Item+Component+Details+Report_1013416_115_1+(5).xlsx&quot;);
            //Get the pivot table 
            PivotTable pivot = workbook.Worksheets[1].PivotTables[0];
            //get row PivotField collection 
            PivotFieldCollection rows = pivot.RowFields;
            //get the first PivotField 
            PivotField field = rows[0];

            //set RepeatItemLabels is true 
            field.IsRepeatItemLabels = true;

            pivot.RefreshData();
            pivot.CalculateData();
            pivot.RefreshDataOnOpeningFile = false;
            cells = workbook.Worksheets[1].Cells;
            Assert.AreEqual(cells[&quot;A10&quot;].StringValue, &quot;Vision Operations&quot;);
            Assert.AreEqual(cells[&quot;A11&quot;].StringValue, &quot;Vision Operations&quot;);

            Assert.AreEqual(cells[&quot;B11&quot;].StringValue, &quot;13612&quot;);
            Assert.AreEqual(cells[&quot;B12&quot;].StringValue, &quot;13612&quot;);


            workbook.Save(Constants.PivotTableDestPath + @&quot;JAVA41551out.xlsx&quot;);
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


