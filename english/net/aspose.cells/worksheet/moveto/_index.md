---
title: Worksheet.MoveTo
second_title: Aspose.Cells for .NET API Reference
description: Worksheet method. Moves the sheet to another location in the spreadsheet
type: docs
url: /net/aspose.cells/worksheet/moveto/
---
## Worksheet.MoveTo method

Moves the sheet to another location in the spreadsheet.

```csharp
public void MoveTo(int index)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | Destination sheet index. |

### Examples

```csharp
// Called: _workBook.Worksheets[_copiedWorkSheetName].MoveTo(0);
[Test]
        public void Method_Int32_()
        {
            string _sourceWorkSheetName = "MySheet";
            string _copiedWorkSheetName = "MyCopiedSheet";
            Workbook _workBook = new Workbook(Constants.sourcePath + "MyExcelFile.xls");
            if (_workBook.Worksheets[_copiedWorkSheetName] == null)
                _workBook.Worksheets.Add(_copiedWorkSheetName);

            _workBook.Worksheets[_copiedWorkSheetName].Copy(_workBook.Worksheets[_sourceWorkSheetName]);
            _workBook.Worksheets[_copiedWorkSheetName].IsVisible = true;

            // This single line make the comment disapears
            _workBook.Worksheets[_copiedWorkSheetName].MoveTo(0);

            Worksheet _workSheet = _workBook.Worksheets[_copiedWorkSheetName];
            int commentIndex = _workSheet.Comments.Add(1, 1);
            _workSheet.Comments[commentIndex].AutoSize = true;
            _workSheet.Comments[commentIndex].Note = "My comment";

            _workBook.Save(Constants.destPath + "OutputCommentFromCopiedAndMovedWorksheet.xls");
            _workBook = new Workbook(Constants.destPath + "OutputCommentFromCopiedAndMovedWorksheet.xls");
            Assert.AreEqual(_workBook.Worksheets[_copiedWorkSheetName].Comments.Count, 1);

        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


