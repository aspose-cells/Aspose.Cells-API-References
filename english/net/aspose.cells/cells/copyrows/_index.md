---
title: Cells.CopyRows
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Copies data and formats of some whole rows
type: docs
url: /net/aspose.cells/cells/copyrows/
---
## CopyRows(Cells, int, int, int) {#copyrows}

Copies data and formats of some whole rows.

```csharp
public void CopyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells | Cells | Source Cells object contains data and formats to copy. |
| sourceRowIndex | Int32 | Source row index. |
| destinationRowIndex | Int32 | Destination row index. |
| rowNumber | Int32 | The copied row number. |

### Examples

```csharp
// Called: worksheet.Cells.CopyRows(worksheet.Cells, 0, 25, 24); // See sheet1 row 25
[Test]
        // Charts not copying correctly
        // http://www.aspose.com/community/forums/thread/293128.aspx
        public void Method_Int32_()
        {
            Console.WriteLine(&quot;Method_Int32_()&quot;);
            string infn = path + @&quot;CELLSNET-25555\ChartTest.xlsx&quot;;
            string outfn = Constants.destPath + @&quot;CELLSNET-25555_out.xlsx&quot;;

            Workbook workbook = new Workbook(infn);
            Worksheet worksheet = workbook.Worksheets[0];
            workbook.Worksheets.AddCopy(0);  // See sheet5
            worksheet.Cells.CopyRows(worksheet.Cells, 0, 25, 24); // See sheet1 row 25
            workbook.Save(outfn, SaveFormat.Xlsx);

            //Console.WriteLine(&quot;Please wait..., This test will open the output file for checking: Charts Copy.&quot;);
            //Process.Start(&quot;explorer.exe&quot;, string.Format(&quot;\&quot;{0}\&quot;&quot;, outfn));
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyRows(Cells, int, int, int, CopyOptions) {#copyrows_1}

Copies data and formats of some whole rows.

```csharp
public void CopyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, 
    int rowNumber, CopyOptions copyOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells0 | Cells | Source Cells object contains data and formats to copy. |
| sourceRowIndex | Int32 | Source row index. |
| destinationRowIndex | Int32 | Destination row index. |
| rowNumber | Int32 | The copied row number. |
| copyOptions | CopyOptions | The copy options. |

### Examples

```csharp
// Called: cells.CopyRows(cells, 0, 1, 1, co);
[Test]
        public void Method_CopyOptions_()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CellsNet45314.xlsx&quot;);

            Worksheet ws = wb.Worksheets[&quot;Sheet1&quot;];

            HyperlinkCollection hyps = ws.Hyperlinks;

            int cnt1 = hyps.Count;

            CopyOptions co = new CopyOptions();
            co.ExtendToAdjacentRange = true;

            Cells cells = ws.Cells;
            cells.CopyRows(cells, 0, 1, 1, co);

            int cnt2 = hyps.Count;
           Assert.AreEqual(1,cnt2);
        }
```

### See Also

* class [CopyOptions](../../copyoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyRows(Cells, int, int, int, CopyOptions, PasteOptions) {#copyrows_2}

Copies data and formats of some whole rows.

```csharp
public void CopyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, 
    int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells0 | Cells | Source Cells object contains data and formats to copy. |
| sourceRowIndex | Int32 | Source row index. |
| destinationRowIndex | Int32 | Destination row index. |
| rowNumber | Int32 | The copied row number. |
| copyOptions | CopyOptions | The copy options. |
| pasteOptions | PasteOptions | the options of pasting. |

### See Also

* class [CopyOptions](../../copyoptions/)
* class [PasteOptions](../../pasteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


