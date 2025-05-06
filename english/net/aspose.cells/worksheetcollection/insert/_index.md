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
// Called: wb.Worksheets.Insert(1, wb.Worksheets[0].Type);
[Test]
        public void Method_SheetType_()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET47024_&quot;;

            Workbook wb = new Workbook(filePath + &quot;Sample.xlsx&quot;);

            wb.Worksheets.Insert(1, wb.Worksheets[0].Type);
            wb.Worksheets[1].Copy(wb.Worksheets[0]);
            Assert.AreEqual(wb.Worksheets[1].PivotTables[0].DataField.Position, 2);
            wb.Save(CreateFolder(filePath) + &quot;out.xlsx&quot;, SaveFormat.Xlsx);
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
// Called: book.Worksheets.Insert(0, SheetType.Worksheet, &amp;quot;insert&amp;quot;);
[Test]
        //http://www.aspose.com/community/forums/thread/221542.aspx
        public void Method_String_()
        {
            Console.WriteLine(&quot;Method_String_()&quot;);
            string infn = path + &quot;Test_CopyButtonWithMacro.xltm&quot;;
            string outfn = Constants.destPath + &quot;Test_CopyButtonWithMacro_out.xlsm&quot;;

            Workbook book = new Workbook(infn);
            book.Worksheets.Insert(0, SheetType.Worksheet, &quot;insert&quot;);
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


