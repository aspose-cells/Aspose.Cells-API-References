---
title: NameCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: NameCollection property. Gets the Name element at the specified index
type: docs
url: /net/aspose.cells/namecollection/item/
---
## NameCollection indexer (1 of 2)

Gets the [`Name`](../../name/) element at the specified index.

```csharp
public Name this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp
// Called: Name name = workbook.Worksheets.Names[rangeIndex];
[Test]
        public void Property_Int32_()
        {
            String dynamicRange = &quot;&apos;Projects&apos;!B4:E19&quot;;
            String worksheetName = &quot;Projects&quot;;
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSJAVA41603.xlsx&quot;);
            Worksheet worksheet = workbook.Worksheets[worksheetName];

            int rangeIndex = workbook.Worksheets.Names.Add(&quot;dummyrange&quot;);
            Name name = workbook.Worksheets.Names[rangeIndex];
            name.RefersTo = dynamicRange;
            name = workbook.Worksheets.Names[rangeIndex];
            Aspose.Cells.Range sourceRange = name.GetRange();

            Workbook newWorkbook = new Workbook(FileFormatType.Xlsx);
            WorksheetCollection targetWsc = newWorkbook.Worksheets;
            Worksheet targetWs = (Worksheet)targetWsc[0];

            Aspose.Cells.Range targetRange = targetWs.Cells.CreateRange(0, 0, sourceRange.RowCount, sourceRange.ColumnCount);

            PasteOptions options = new PasteOptions();

            //Copy column widths
            options.PasteType = PasteType.ColumnWidths;
            targetRange.Copy(sourceRange, options);

            // Copy row heights
            int rowCount = sourceRange.RowCount;
            int firstRow = sourceRange.FirstRow;
            for (int i = 0; i &lt; rowCount; i++)
            {
                double rowHeight = sourceRange.Worksheet.Cells.GetRowHeight(firstRow++);
                targetWs.Cells.SetRowHeight(i, rowHeight);
            }

            //Copy everything else
            options.PasteType = PasteType.All;

            targetRange.Copy(sourceRange, options);

            Util.ReSave(newWorkbook, SaveFormat.Xlsx);
            //newWorkbook.Save(Constants.destPath + &quot;CELLSJAVA41603.xlsx&quot;);
            AssertHelper.AreEqual(workbook.Worksheets[&quot;Projects&quot;].Cells[&quot;C4&quot;].GetStyle().ForegroundColor,
                newWorkbook.Worksheets[0].Cells[&quot;B1&quot;].GetStyle().ForegroundColor);
        }
```

### See Also

* class [Name](../../name/)
* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## NameCollection indexer (2 of 2)

Gets the [`Name`](../../name/) element with the specified name.

```csharp
public Name this[string text] { get; }
```

| Parameter | Description |
| --- | --- |
| text | Name text. |

### Return Value

The element with the specified name.

### Examples

```csharp
// Called: Name namedRange = workbook.Worksheets.Names[&amp;quot;RowRanges.R3&amp;quot;];
[Test, Category(&quot;Bug&quot;)]
        public void Property_String_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;SpecialCharactersSheetNames.xls&quot;);
            Worksheet worksheet = workbook.Worksheets[0];
            Name namedRange = workbook.Worksheets.Names[&quot;RowRanges.R3&quot;];
            namedRange.RefersTo = string.Format(&quot;=&apos;{0}&apos;!$1:$2&quot;, worksheet.Name);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
        }
```

### See Also

* class [Name](../../name/)
* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


