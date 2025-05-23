---
title: OdsCellField.FieldType
second_title: Aspose.Cells for .NET API Reference
description: OdsCellField property. Gets and sets the type of the field
type: docs
url: /net/aspose.cells.ods/odscellfield/fieldtype/
---
## OdsCellField.FieldType property

Gets and sets the type of the field.

```csharp
public OdsCellFieldType FieldType { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(OdsCellFieldType.Title, sheet.Cells.OdsCellFields[0].FieldType);
public void OdsCellField_Property_FieldType()
 {
     Workbook workbook = new Workbook(Constants.sourcePath + "example.ods");
     Worksheet sheet = workbook.Worksheets[0];
     Assert.AreEqual(OdsCellFieldType.Title, sheet.Cells.OdsCellFields[0].FieldType);
     Assert.AreEqual(OdsCellFieldType.SheetName, sheet.Cells.OdsCellFields[1].FieldType);
     workbook.Save(Constants.destPath + "example.ods");
     workbook = new Workbook(Constants.destPath + "example.ods");
     sheet = workbook.Worksheets[0];
     Assert.AreEqual(OdsCellFieldType.Title, sheet.Cells.OdsCellFields[0].FieldType);
     Assert.AreEqual(OdsCellFieldType.SheetName, sheet.Cells.OdsCellFields[1].FieldType);
 }
```

### See Also

* enum [OdsCellFieldType](../../odscellfieldtype/)
* class [OdsCellField](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


