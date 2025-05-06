---
title: Cell.GetCharacters
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Returns all Characters objects that represents a range of characters within the cell text
type: docs
url: /net/aspose.cells/cell/getcharacters/
---
## GetCharacters() {#getcharacters}

Returns all Characters objects that represents a range of characters within the cell text.

```csharp
public FontSetting[] GetCharacters()
```

### Return Value

All Characters objects

### Examples

```csharp
// Called: Assert.AreEqual(a1.GetCharacters()[0].Font.IsBold, true);
[Test]
        public void Method_GetCharacters()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;NET45195/&quot;;
            //HtmlLoadOptions opt = new HtmlLoadOptions(LoadFormat.Html);
            //opt.AutoFitColsAndRows = true;
            //Workbook workbook = new Workbook(filePath + &quot;EditorToHtml-NotWorking-1.html&quot;, opt);
            //workbook.Save(CreateFolder(filePath) + &quot;out1.xlsx&quot;);
            //workbook = new Workbook(filePath + &quot;EditorToHtml-NotWorking-2.html&quot;, opt);
            //workbook.Save(CreateFolder(filePath) + &quot;out2.xlsx&quot;);

            HtmlLoadOptions opt = new HtmlLoadOptions(LoadFormat.Html);
            opt.AutoFitColsAndRows = true;
            Workbook workbook = null;
            Cells cells = null;
            Cell a1 = null;
            workbook = new Workbook(filePath + &quot;EditorToHtml-NotWorking-1.html&quot;, opt);
            cells = workbook.Worksheets[0].Cells;
           // Console.WriteLine(cells.MergedCells.Count);
            Assert.AreEqual(cells.GetMergedAreas().Length, 14);
            a1 = cells[&quot;A1&quot;];
            Assert.AreEqual(a1.IsRichText(), false);
            Assert.AreEqual(a1.GetStyle().Font.IsBold, true);

            Assert.AreEqual(cells[&quot;A8&quot;].IsRichText(), false);
            Assert.AreEqual(cells[&quot;A8&quot;].GetStyle().Font.IsBold, true);

            Assert.AreEqual(cells[&quot;A12&quot;].IsRichText(), false);
            Assert.AreEqual(cells[&quot;A12&quot;].GetStyle().Font.IsBold, true);

            Assert.AreEqual(cells[&quot;A15&quot;].IsRichText(), true);
            Assert.AreEqual(cells[&quot;A15&quot;].GetCharacters()[2].Font.Color, Color.FromArgb(255, 255, 0, 0));

            workbook.Save(CreateFolder(filePath) + &quot;out1.xlsx&quot;);

            workbook = new Workbook(filePath + &quot;EditorToHtml-NotWorking-2.html&quot;, opt);
            cells = workbook.Worksheets[0].Cells;
           
            Assert.AreEqual(cells.GetMergedAreas().Length, 16);
            a1 = cells[&quot;A1&quot;];
            Assert.AreEqual(a1.IsRichText(), true);
            Assert.AreEqual(a1.GetCharacters().Length, 11);
            Assert.AreEqual(a1.GetCharacters()[0].Font.IsBold, true);
            Assert.AreEqual(a1.GetCharacters()[3].Font.Color, Color.FromArgb(255, 255, 0, 0));
            Assert.AreEqual(a1.GetCharacters()[8].Font.Color, Color.FromArgb(255, 255, 0, 0));
            Assert.AreEqual(a1.GetCharacters()[5].Font.Color, Color.FromArgb(255, 79, 129, 189));

            Assert.AreEqual(cells[&quot;A2&quot;].IsRichText(), true);
            Assert.AreEqual(cells[&quot;A2&quot;].GetCharacters()[0].Font.IsBold, true);
            Assert.AreEqual(cells[&quot;A3&quot;].IsRichText(), true);
            Assert.AreEqual(cells[&quot;A3&quot;].GetCharacters()[0].Font.IsBold, true);

            workbook.Save(CreateFolder(filePath) + &quot;out2.xlsx&quot;);
        }
```

### See Also

* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetCharacters(bool) {#getcharacters_1}

Returns all Characters objects that represents a range of characters within the cell text.

```csharp
public FontSetting[] GetCharacters(bool flag)
```

| Parameter | Type | Description |
| --- | --- | --- |
| flag | Boolean | Indicates whether applying table style to the cell if the cell is in the table. |

### Return Value

All Characters objects

### Examples

```csharp
// Called: FontSetting[] fs = cell.GetCharacters(true);
[Test]
        public void Method_Boolean_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet44480.xlsx&quot;);
            Cell cell = workbook.Worksheets[0].Cells[&quot;C8&quot;];
            FontSetting[] fs = cell.GetCharacters(true);
            for (int i = 0; i &lt; fs.Length; i++)
            {
               AssertHelper.AreEqual(Color.White, fs[i].Font.Color);
            }
        }
```

### See Also

* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


