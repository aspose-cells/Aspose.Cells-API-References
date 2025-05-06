---
title: HyperlinkCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: HyperlinkCollection method. Adds a hyperlink to a specified cell or a range of cells
type: docs
url: /net/aspose.cells/hyperlinkcollection/add/
---
## Add(int, int, int, int, string) {#add}

Adds a hyperlink to a specified cell or a range of cells.

```csharp
public int Add(int firstRow, int firstColumn, int totalRows, int totalColumns, string address)
```

| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | First row of the hyperlink range. |
| firstColumn | Int32 | First column of the hyperlink range. |
| totalRows | Int32 | Number of rows in this hyperlink range. |
| totalColumns | Int32 | Number of columns of this hyperlink range. |
| address | String | Address of the hyperlink. |

### Return Value

[`Hyperlink`](../../hyperlink/) object index.

### Examples

```csharp
[C#]
//Instantiating a Workbook object
Workbook excel = new Workbook();
Worksheet worksheet = excel.Worksheets[0];
worksheet.Hyperlinks.Add("A4", 1, 1, "http://www.aspose.com");
worksheet.Hyperlinks.Add("A5", 1, 1, "c:\\book1.xls");

[Visual Basic]

'Instantiating a Workbook object
Dim excel As Workbook = New Workbook()
Dim worksheet as Worksheet = excel.Worksheets(0)
worksheet.Hyperlinks.Add("A4", 1, 1, "http://www.aspose.com")
worksheet.Hyperlinks.Add("A5", 1, 1, "c:\\book1.xls")

```

### See Also

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int, string) {#add_1}

Adds a hyperlink to a specified cell or a range of cells.

```csharp
public int Add(string cellName, int totalRows, int totalColumns, string address)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | Cell name. |
| totalRows | Int32 | Number of rows in this hyperlink range. |
| totalColumns | Int32 | Number of columns of this hyperlink range. |
| address | String | Address of the hyperlink. |

### Return Value

[`Hyperlink`](../../hyperlink/) object index.

### Examples

```csharp
// Called: workbook.Worksheets[0].Hyperlinks.Add(&amp;quot;A5&amp;quot;, 1, 1, &amp;quot;Book1.xlsx#sheet1!A1&amp;quot;);
[Test]
        public void Method_String_()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Hyperlinks.Add(&quot;A5&quot;, 1, 1, &quot;Book1.xlsx#sheet1!A1&quot;);
            workbook.Save(Constants.destPath + &quot;CellsJava41010.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsJava41010.xlsx&quot;);
            Assert.AreEqual(workbook.Worksheets[0].Hyperlinks[0].Address, &quot;Book1.xlsx#sheet1!A1&quot;);
        }
```

### See Also

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string, string, string) {#add_2}

Adds a hyperlink to a specified cell or a range of cells.

```csharp
public int Add(string startCellName, string endCellName, string address, string textToDisplay, 
    string screenTip)
```

| Parameter | Type | Description |
| --- | --- | --- |
| startCellName | String | The top-left cell of the range. |
| endCellName | String | The bottom-right cell of the range. |
| address | String | Address of the hyperlink. |
| textToDisplay | String | The text to be displayed for the specified hyperlink. |
| screenTip | String | The screenTip text for the specified hyperlink. |

### Return Value

[`Hyperlink`](../../hyperlink/) object index.

### Examples

```csharp
// Called: hyperlinks.Add(&amp;quot;D1&amp;quot;, &amp;quot;D2&amp;quot;, &amp;quot;http://www.display.com&amp;quot;, &amp;quot;Click Here&amp;quot;, &amp;quot;Go to Display&amp;quot;);
public static void Method_String_()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();

            // Obtaining the reference of the newly added worksheet by passing its sheet index
            Worksheet worksheet = workbook.Worksheets[0];

            // Get Hyperlinks Collection
            HyperlinkCollection hyperlinks = worksheet.Hyperlinks;

            // Adding a hyperlink to a URL at &quot;A1&quot; cell
            hyperlinks.Add(&quot;A1&quot;, 1, 1, &quot;http://www.aspose.com&quot;);

            // Adding another hyperlink to a URL at &quot;B1&quot; cell
            hyperlinks.Add(&quot;B1&quot;, 1, 1, &quot;http://www.example.com&quot;);

            // Adding a hyperlink with a range of cells
            hyperlinks.Add(&quot;C1&quot;, 1, 2, &quot;http://www.test.com&quot;);

            // Adding a hyperlink with a specific text to display and screen tip
            hyperlinks.Add(&quot;D1&quot;, &quot;D2&quot;, &quot;http://www.display.com&quot;, &quot;Click Here&quot;, &quot;Go to Display&quot;);

            // Removing the first hyperlink
            hyperlinks.RemoveAt(0);

            // Clearing all hyperlinks
            hyperlinks.Clear();

            // Adding a hyperlink again to demonstrate saving
            hyperlinks.Add(&quot;A1&quot;, 1, 1, &quot;http://www.aspose.com&quot;);

            // Saving the Excel file
            workbook.Save(&quot;HyperlinkCollectionExample.xlsx&quot;);
            workbook.Save(&quot;HyperlinkCollectionExample.pdf&quot;);
            return;
        }
```

### See Also

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


