---
title: FindOptions.SearchBackward
second_title: Aspose.Cells for .NET API Reference
description: FindOptions property. Whether search backward for cells
type: docs
url: /net/aspose.cells/findoptions/searchbackward/
---
## FindOptions.SearchBackward property

Whether search backward for cells.

```csharp
public bool SearchBackward { get; set; }
```

### Examples

```csharp
// Called: findOptions.SearchBackward = false;
[Test]
        public void Property_SearchBackward()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "TestCELLSNET_12550.xls");
            Cells cells = workbook.Worksheets[0].Cells;
            FindOptions findOptions = new FindOptions();
            CellArea ca = new CellArea();
            ca.StartRow = 8;
            ca.StartColumn = 2;
            ca.EndRow = 17;
            ca.EndColumn = 13;
            findOptions.SetRange(ca);
            //  
            //Cell cell = cells.Find(0, cells["D9"], findOptions);
            findOptions.SearchBackward = false;
            findOptions.SearchOrderByRows = true;
            findOptions.LookInType = LookInType.Values;
            Cell cell = cells.Find(0, null, findOptions);
            Assert.AreEqual(cell.Name, "C9");
        }
```

### See Also

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


