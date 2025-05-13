---
title: WorksheetCollection.Insert
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection method. Insert a worksheet
type: docs
url: /net/aspose.cells/worksheetcollection/insert/
---
## Insert(int, SheetType) {#insert}

Insert a worksheet.

```csharp
public Worksheet Insert(int index, SheetType sheetType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The sheet index |
| sheetType | SheetType | The sheet type. |

### Return Value

Returns an inserted worksheet.

### Examples

```csharp
// Called: Worksheet worksheet =  workbook.Worksheets.Insert(1, SheetType.Worksheet);
[Test, Category("Bug")]
        public void WorksheetCollection_Method_Insert()
        {
            Workbook workbook = new Workbook();
           Worksheet worksheet =  workbook.Worksheets.Insert(1, SheetType.Worksheet);
           worksheet.Name = "mm-mm";
           workbook.Worksheets[0].Cells["A1"].Formula = "='mm-mm'!A1";
        }
```

### See Also

* class [Worksheet](../../worksheet/)
* enum [SheetType](../../sheettype/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Insert(int, SheetType, string) {#insert_1}

Insert a worksheet.

```csharp
public Worksheet Insert(int index, SheetType sheetType, string sheetName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The sheet index |
| sheetType | SheetType | The sheet type. |
| sheetName | String | The sheet name. |

### Return Value

Returns an inserted worksheet.

### Examples

```csharp
// Called: book.Worksheets.Insert(0, SheetType.Worksheet, "insert");
//http://www.aspose.com/community/forums/thread/221542.aspx
public void WorksheetCollection_Method_Insert()
{
    Console.WriteLine("WorksheetCollection_Method_Insert()");
    string infn = path + "Test_CopyButtonWithMacro.xltm";
    string outfn = Constants.destPath + "Test_CopyButtonWithMacro_out.xlsm";

    Workbook book = new Workbook(infn);
    book.Worksheets.Insert(0, SheetType.Worksheet, "insert");
    Worksheet sheet = book.Worksheets[0];
    sheet.Copy(book.Worksheets[1]);
    book.Save(outfn);
}
```

### See Also

* class [Worksheet](../../worksheet/)
* enum [SheetType](../../sheettype/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


