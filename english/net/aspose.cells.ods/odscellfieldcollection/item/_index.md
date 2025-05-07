---
title: OdsCellFieldCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: OdsCellFieldCollection property. Gets the field by the index
type: docs
url: /net/aspose.cells.ods/odscellfieldcollection/item/
---
## OdsCellFieldCollection indexer (1 of 2)

Gets the field by the index.

```csharp
public OdsCellField this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index. |

### Examples

```csharp
// Called: Assert.AreEqual(OdsCellFieldType.Title, sheet.Cells.OdsCellFields[0].FieldType);
[Test]
       public void Property_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET48653.ods");
            Worksheet sheet = workbook.Worksheets[0];
            Assert.AreEqual(OdsCellFieldType.Title, sheet.Cells.OdsCellFields[0].FieldType);
            Assert.AreEqual(OdsCellFieldType.SheetName, sheet.Cells.OdsCellFields[1].FieldType);
            workbook.Save(Constants.destPath + "CELLSNET48653.ods");
            workbook = new Workbook(Constants.destPath + "CELLSNET48653.ods");
            sheet = workbook.Worksheets[0];
            Assert.AreEqual(OdsCellFieldType.Title, sheet.Cells.OdsCellFields[0].FieldType);
            Assert.AreEqual(OdsCellFieldType.SheetName, sheet.Cells.OdsCellFields[1].FieldType);
        }
```

### See Also

* class [OdsCellField](../../odscellfield/)
* class [OdsCellFieldCollection](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)

---

## OdsCellFieldCollection indexer (2 of 2)

Gets the field by row and column index.

```csharp
public OdsCellField this[int row, int column] { get; }
```

| Parameter | Description |
| --- | --- |
| row | The row index. |
| column | The column index. |

### See Also

* class [OdsCellField](../../odscellfield/)
* class [OdsCellFieldCollection](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


