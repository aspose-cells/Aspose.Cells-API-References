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
// Called: links.Add("A1", 1, 1, "www.aspose.com");
public void HyperlinkCollection_Method_Add()
{
    Workbook w = new Workbook();
    HyperlinkCollection links = w.Worksheets[0].Hyperlinks;
    links.Add("A1", 1, 1, "www.aspose.com");
    Assert.AreEqual("www.aspose.com", w.Worksheets[0].Cells["A1"].StringValue);
    w.Worksheets[0].Cells["A1"].PutValue("sdfsdf");
    Assert.AreEqual("sdfsdf", links[0].TextToDisplay);
    w.Save(Constants.destPath + "example.xlsx");
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
// Called: hyperlinks.Add("D1", "D2", "http://www.display.com", "Click Here", "Go to Display");
public static void HyperlinkCollection_Method_Add()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();

            // Obtaining the reference of the newly added worksheet by passing its sheet index
            Worksheet worksheet = workbook.Worksheets[0];

            // Get Hyperlinks Collection
            HyperlinkCollection hyperlinks = worksheet.Hyperlinks;

            // Adding a hyperlink to a URL at "A1" cell
            hyperlinks.Add("A1", 1, 1, "http://www.aspose.com");

            // Adding another hyperlink to a URL at "B1" cell
            hyperlinks.Add("B1", 1, 1, "http://www.example.com");

            // Adding a hyperlink with a range of cells
            hyperlinks.Add("C1", 1, 2, "http://www.test.com");

            // Adding a hyperlink with a specific text to display and screen tip
            hyperlinks.Add("D1", "D2", "http://www.display.com", "Click Here", "Go to Display");

            // Removing the first hyperlink
            hyperlinks.RemoveAt(0);

            // Clearing all hyperlinks
            hyperlinks.Clear();

            // Adding a hyperlink again to demonstrate saving
            hyperlinks.Add("A1", 1, 1, "http://www.aspose.com");

            // Saving the Excel file
            workbook.Save("HyperlinkCollectionExample.xlsx");
            workbook.Save("HyperlinkCollectionExample.pdf");
            return;
        }
```

### See Also

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


