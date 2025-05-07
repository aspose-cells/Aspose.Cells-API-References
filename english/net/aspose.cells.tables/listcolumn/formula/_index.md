---
title: ListColumn.Formula
second_title: Aspose.Cells for .NET API Reference
description: ListColumn property. Gets and sets the formula of the list column
type: docs
url: /net/aspose.cells.tables/listcolumn/formula/
---
## ListColumn.Formula property

Gets and sets the formula of the list column.

```csharp
public string Formula { get; set; }
```

### Examples

```csharp
// Called: listObject.ListColumns[1].Formula = fml;
[Test]
        public void Property_Formula()
        {
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];

            sheet.Cells[0, 0].PutValue("Column A");
            sheet.Cells[0, 1].PutValue("Column B");

            ListObject listObject =
              sheet.ListObjects[sheet.ListObjects.Add(0, 0, 1, sheet.Cells.MaxColumn, true)];
            listObject.TableStyleType = TableStyleType.TableStyleMedium2;
            listObject.DisplayName = "Table";
            string fml = "=[Column A] + 1";
            listObject.ListColumns[1].Formula = fml;
            Assert.AreEqual(book.Settings.FormulaSettings.PreservePaddingSpaces
                ? "=[Column A] + 1" : "=[Column A]+1", sheet.Cells["B2"].Formula);
            book = Util.ReSave(book, SaveFormat.Xlsx);
        }
```

### See Also

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


