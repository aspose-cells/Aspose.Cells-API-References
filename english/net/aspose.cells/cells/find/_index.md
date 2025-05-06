---
title: Cells.Find
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Finds the cell containing with the input object
type: docs
url: /net/aspose.cells/cells/find/
---
## Find(object, Cell) {#find}

Finds the cell containing with the input object.

```csharp
public Cell Find(object what, Cell previousCell)
```

| Parameter | Type | Description |
| --- | --- | --- |
| what | Object | The object to search for. The type should be int,double,DateTime,string,bool. |
| previousCell | Cell | Previous cell with the same object. This parameter can be set to null if searching from the start. |

### Return Value

Cell object.

### Remarks

Returns null (Nothing) if no cell is found.

### Examples

```csharp
// Called: cell = worksheet.Cells.Find(&amp;quot;Grand Total&amp;quot;, null);
[Test]
        public void Method_Cell_()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;JAVA44632_&quot;;

            Workbook wb = new Workbook(filePath + &quot;a.xlsx&quot;);
            Worksheet worksheet = wb.Worksheets[1];
            PivotTable pivotTable = worksheet.PivotTables[0];
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            //Create the style with your desired formatting
            Style style = wb.CreateStyle();
            style.Custom = &quot;0.00%&quot;;
            style.Font.Name = &quot;Calibri&quot;;
            style.Font.Size = 11;

            //Find the cell containing the row field text/label
            Cell cell = worksheet.Cells.Find(&quot;Other Adj.&quot;, null);

            pivotTable.FormatRow(cell.Row, style);

            cell = worksheet.Cells.Find(&quot;Grand Total&quot;, null);
            pivotTable.FormatRow(cell.Row, style);
            wb.Save(Constants.PivotTableDestPath + &quot;JAVA44632.html&quot;);
            Assert.AreNotEqual(worksheet.Cells[&quot;B8&quot;].StringValue.IndexOf(&quot;%&quot;), -1);
            Assert.AreNotEqual(worksheet.Cells[&quot;B48&quot;].StringValue.IndexOf(&quot;%&quot;), -1);
         
        }
```

### See Also

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Find(object, Cell, FindOptions) {#find_1}

Finds the cell containing with the input object.

```csharp
public Cell Find(object what, Cell previousCell, FindOptions findOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| what | Object | The object to search for. The type should be int,double,DateTime,string,bool. |
| previousCell | Cell | Previous cell with the same object. This parameter can be set to null if searching from the start. |
| findOptions | FindOptions | Find options |

### Return Value

Cell object.

### Remarks

Returns null (Nothing) if no cell is found.

### Examples

```csharp
// Called: Cell cell = cells.Find(formula, previousCell, new FindOptions()
private void Method_FindOptions_(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            Cell previousCell = cells[1, 3];
            string formula = &quot;=SUM(A1,B1)&quot;;
            Cell cell = cells.Find(formula, previousCell, new FindOptions()
            { LookInType = LookInType.OnlyFormulas, LookAtType = LookAtType.Contains });
            testAreEqual(3, cell.Row, caseName);
            testAreEqual(5, cell.Column, caseName);
        }
```

### See Also

* class [Cell](../../cell/)
* class [FindOptions](../../findoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


