---
title: Cells.DeleteColumn
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Deletes a column
type: docs
url: /net/aspose.cells/cells/deletecolumn/
---
## DeleteColumn(int, bool) {#deletecolumn_1}

Deletes a column.

```csharp
public void DeleteColumn(int columnIndex, bool updateReference)
```

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Index of the column to be deleted. |
| updateReference | Boolean | Indicates whether update references in other worksheets. |

### Examples

```csharp
// Called: cells.DeleteColumn(5, true);
[Test]
        public void Method_Boolean_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Test_188980.xlsx&quot;);
            Cells cells = workbook.Worksheets[0].Cells;
            cells.DeleteColumn(1, true);
            cells.DeleteColumn(5, true);
            cells.DeleteRow(0);
            cells.DeleteRow(5);
            Assert.AreEqual(&quot;B1:E8&quot;, workbook.Worksheets[0].PageSetup.PrintArea, &quot;PrintArea&quot;);

        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteColumn(int) {#deletecolumn}

Deletes a column.

```csharp
public void DeleteColumn(int columnIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Index of the column to be deleted. |

### Examples

```csharp
// Called: cells.DeleteColumn(0);
[Test]
        public void Method_Int32_()
        {
            caseName = &quot;testDeleteFormual_005&quot;;
            Workbook workbook = new Workbook();
            workbook = new Workbook(Constants.sourcePath + &quot;insertDelete\\testformual2.xls&quot;);
            Cells cells = workbook.Worksheets[0].Cells;
            cells.DeleteColumn(0);

            checkDeleteFormual_005(workbook);
            workbook.Save(Constants.destPath + &quot;testDeleteFormual.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot;testDeleteFormual.xls&quot;);
            checkDeleteFormual_005(workbook);
            workbook.Save(Constants.destPath + &quot;testDeleteFormual.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;testDeleteFormual.xlsx&quot;);
            checkDeleteFormual_005(workbook);
            workbook.Save(Constants.destPath + &quot;testDeleteFormual.xml&quot;, SaveFormat.SpreadsheetML);
            workbook = new Workbook(Constants.destPath + &quot;testDeleteFormual.xml&quot;);
            checkDeleteFormual_005(workbook);
            workbook.Save(Constants.destPath + &quot;testDeleteFormual.xls&quot;);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


