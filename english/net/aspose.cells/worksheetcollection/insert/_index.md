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
// Called: loOrigWB.Worksheets.Insert(0, SheetType.Worksheet).Copy(loOrigWS);
[Test]
        public void Method_SheetType_()
        {
            string filePath = Constants.PivotTableSourcePath + @"NET46587_";

            Workbook loOrigWB = new Workbook(filePath + @"Orig.xlsx");
            Worksheet loOrigWS = loOrigWB.Worksheets["Sheet1"];
            loOrigWB.Worksheets.Insert(0, SheetType.Worksheet).Copy(loOrigWS);
            var loNewWS = loOrigWB.Worksheets["Sheet2"];
            loNewWS.Cells.DeleteRows(0, 3);
            loNewWS.Cells.DeleteColumns(0, 3, true);
            loNewWS.RefreshPivotTables();
            loNewWS.Charts[0].RefreshPivotData();
            loOrigWB.Save(Constants.PIVOT_CHECK_FILE_PATH + @"NET46587.xlsx");
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
[Test]
        //http://www.aspose.com/community/forums/thread/221542.aspx
        public void Method_String_()
        {
            Console.WriteLine("Method_String_()");
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


