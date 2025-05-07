---
title: Workbook.CellsDataTableFactory
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Gets the factory for building ICellsDataTable from custom objects
type: docs
url: /net/aspose.cells/workbook/cellsdatatablefactory/
---
## Workbook.CellsDataTableFactory property

Gets the factory for building ICellsDataTable from custom objects

```csharp
public CellsDataTableFactory CellsDataTableFactory { get; }
```

### Examples

```csharp
// Called: ICellsDataTable dt = wb.CellsDataTableFactory.GetInstance(dataLists, true);
[Test]
        public void Property_CellsDataTableFactory()
        {
            Workbook wb = new Workbook();

            ArrayList dataLists = new ArrayList();
            dataLists.Add(new object[] { "Name", "Age", "Gender" });
            dataLists.Add(new object[] { "Alice", 30, "Female" });
            dataLists.Add(new object[] { "Bob", 25, "Male" });
            dataLists.Add(new object[] { "Charlie", 35, "Male" });

            ICellsDataTable dt = wb.CellsDataTableFactory.GetInstance(dataLists, true);

            wb.Worksheets[0].Cells.ImportData(dt, 0, 0, new ImportTableOptions());
            Assert.AreEqual("Alice", wb.Worksheets[0].Cells["A2"].StringValue);

            wb.Worksheets.Add();
            wb.Worksheets[1].Cells.ImportArrayList(dataLists, 0, 0, true);
            Assert.AreEqual("Bob", wb.Worksheets[1].Cells["A3"].StringValue);
        }
```

### See Also

* class [CellsDataTableFactory](../../cellsdatatablefactory/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


