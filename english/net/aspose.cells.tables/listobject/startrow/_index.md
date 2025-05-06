---
title: ListObject.StartRow
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Gets the start row of the range
type: docs
url: /net/aspose.cells.tables/listobject/startrow/
---
## ListObject.StartRow property

Gets the start row of the range.

```csharp
public int StartRow { get; }
```

### Examples

```csharp
// Called: table.Resize(table.StartRow, table.StartColumn, 49, table.EndColumn, true);
[Test]
        public void Property_StartRow()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsJava42021_1.xlsx&quot;);
            Worksheet sheet = workbook.Worksheets[&quot;test&quot;];
            ListObject table = sheet.ListObjects[&quot;Table1&quot;];
            table.Resize(table.StartRow, table.StartColumn, 4, table.EndColumn, true);
            Assert.AreEqual(&quot;=IF(B4,[[If applicable amount of BE calculated using approximation ]],F4+G4+H4)&quot;, sheet.Cells[&quot;E4&quot;].Formula);
            workbook.Save(Constants.destPath + &quot;CellsJava42021_1.xlsx&quot;);

           
            workbook = new Workbook(Constants.sourcePath + &quot;CellsJava42021.xlsx&quot;);
            sheet = workbook.Worksheets[&quot;S.21.01.01&quot;];
            table = sheet.ListObjects[0];
            table.Resize(table.StartRow, table.StartColumn, 49, table.EndColumn, true);
            Assert.AreEqual(&quot;=IF([@Bracket]=\&quot;Bracket 1\&quot;,0,IF([@Bracket]=\&quot;Total\&quot;,\&quot;\&quot;,F32))&quot;, sheet.Cells[&quot;E33&quot;].Formula);
            workbook.Save(Constants.destPath + &quot;CellsJava42021.xlsx&quot;);
        }
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


