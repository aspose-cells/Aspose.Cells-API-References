---
title: ColumnCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ColumnCollection property. Gets a Column object by column index. The Column object of given column index will be instantiated if it does not exist before
type: docs
url: /net/aspose.cells/columncollection/item/
---
## ColumnCollection indexer

Gets a [`Column`](../../column/) object by column index. The Column object of given column index will be instantiated if it does not exist before.

```csharp
public Column this[int columnIndex] { get; }
```

### Examples

```csharp
// Called: double x = workSheet.Cells.Columns[2].Width;
[Test]
        public void Property_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "Cells44049.xlsx");
            Worksheet  workSheet = workbook.Worksheets[0];
            double x = workSheet.Cells.Columns[2].Width;
            workSheet.Cells.Columns[2].IsHidden = true;

            workbook.Save(Constants.destPath + "Cells44049.xlsx");
            workbook = new Workbook(Constants.destPath + "Cells44049.xlsx");
            Assert.AreEqual(x, workbook.Worksheets[0].Cells.Columns[2].Width);


        }
```

### See Also

* class [Column](../../column/)
* class [ColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


