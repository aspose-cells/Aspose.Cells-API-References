---
title: Cells.OdsCellFields
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Gets the list of fields of ods
type: docs
url: /net/aspose.cells/cells/odscellfields/
---
## Cells.OdsCellFields property

Gets the list of fields of ods.

```csharp
public OdsCellFieldCollection OdsCellFields { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[0].Cells.OdsCellFields.Count, 3);
[Test]
        public void Property_OdsCellFields()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsJava42869_1.ods");
            Assert.AreEqual(workbook.Worksheets[0].Cells.OdsCellFields.Count, 3);
            workbook.Save(Constants.destPath + "CellsJava42869.ods");
            workbook  = new Workbook(Constants.destPath + "CellsJava42869.ods");
            Assert.AreEqual(workbook.Worksheets[0].Cells.OdsCellFields.Count, 3);
        }
```

### See Also

* class [OdsCellFieldCollection](../../../aspose.cells.ods/odscellfieldcollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


