---
title: WorksheetCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection property. Gets the Worksheet element at the specified index
type: docs
url: /net/aspose.cells/worksheetcollection/item/
---
## WorksheetCollection indexer (1 of 2)

Gets the [`Worksheet`](../../worksheet/) element at the specified index.

```csharp
public Worksheet this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp
// Called: Cells cellsSrc = wbSrc.Worksheets[0].Cells;
[Test]
        public void Property_Int32_()
        {
            Workbook wbSrc = new Workbook();            
            wbSrc = new Workbook(Constants.sourcePath + &quot;insertDelete\\testformual3.xls&quot;);
            Cells cellsSrc = wbSrc.Worksheets[0].Cells;
            Workbook wbDest = new Workbook();
            Cells cellsDest = wbDest.Worksheets[0].Cells;
            Aspose.Cells.Range rangeSrc = cellsSrc.CreateRange(2, 2, 3, 4);
            Aspose.Cells.Range rangeDest = cellsDest.CreateRange(8, 0, 3, 4);
            rangeDest.CopyValue(rangeSrc);

            checkRangeCopyValue_Formual_001(wbDest);
            wbDest.Save(Constants.destPath + &quot;testRangeCopyValue.xls&quot;);
            wbDest = new Workbook(Constants.destPath + &quot;testRangeCopyValue.xls&quot;);
            checkRangeCopyValue_Formual_001(wbDest);
            wbDest.Save(Constants.destPath + &quot;testRangeCopyValue.xlsx&quot;);
            wbDest = new Workbook(Constants.destPath + &quot;testRangeCopyValue.xlsx&quot;);
            checkRangeCopyValue_Formual_001(wbDest);
            wbDest.Save(Constants.destPath + &quot;testRangeCopyValue.xml&quot;, SaveFormat.SpreadsheetML);
            wbDest = new Workbook(Constants.destPath + &quot;testRangeCopyValue.xml&quot;);
            checkRangeCopyValue_Formual_001(wbDest);
            wbDest.Save(Constants.destPath + &quot;testRangeCopyValue.xls&quot;);
        }
```

### See Also

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## WorksheetCollection indexer (2 of 2)

Gets the [`Worksheet`](../../worksheet/) element with the specified name.

```csharp
public Worksheet this[string sheetName] { get; }
```

| Parameter | Description |
| --- | --- |
| sheetName | Worksheet name |

### Return Value

The element with the specified name.

### Examples

```csharp
// Called: Worksheet sheet = workbook.Worksheets[&amp;quot;Sheet1&amp;quot;];
private void Property_String_(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[&quot;Sheet1&quot;];
            Chart chart = sheet.Charts[0];
            AssertHelper.AreEqual(DataLabelsSeparatorType.Space, chart.NSeries[5].DataLabels.SeparatorType, &quot;chart.NSeries[5].DataLabels.Separator&quot;);
        }
```

### See Also

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


