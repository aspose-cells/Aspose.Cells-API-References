---
title: ListObject.StartColumn
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Gets the start column of the range
type: docs
url: /net/aspose.cells.tables/listobject/startcolumn/
---
## ListObject.StartColumn property

Gets the start column of the range.

```csharp
public int StartColumn { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(table.StartColumn, 5);
public void ListObject_Property_StartColumn()
{
    Workbook wb = new Workbook(SrcPath + "AddXmlMapping.xlsx");
    Worksheet sheet = wb.Worksheets["Merge"];
    Cells cells = sheet.Cells;

    cells.LinkToXmlMap("Transmittals_Map", 6, 5, "/Transmittals/Transmittal_folder/Element/Level");
    cells.LinkToXmlMap("Transmittals_Map", 6, 12, "/Transmittals/Issued_Document");

    Assert.AreEqual(sheet.ListObjects.Count, 1);

    ListObject table = sheet.ListObjects[0];
    Assert.AreEqual(cells["F7"].StringValue, "Level");
    Assert.AreEqual(cells["M7"].StringValue, "Type");
    Assert.AreEqual(cells["N7"].StringValue, "Create_Date");
    Assert.AreEqual(cells["O7"].StringValue, "Create_User");
    Assert.AreEqual(table.StartColumn, 5);
    Assert.AreEqual(table.EndColumn, 14);

    wb.Save(Constants.destPath + "testAddXmlMappingMerge.xlsx");
}
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


