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

### See Also

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


