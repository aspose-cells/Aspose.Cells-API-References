---
title: Cells.LinkToXmlMap
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Link to a xml map
type: docs
url: /net/aspose.cells/cells/linktoxmlmap/
---
## Cells.LinkToXmlMap method

Link to a xml map.

```csharp
public void LinkToXmlMap(string mapName, int row, int column, string path)
```

| Parameter | Type | Description |
| --- | --- | --- |
| mapName | String | name of xml map |
| row | Int32 | row of the destination cell |
| column | Int32 | column of the destination cell |
| path | String | path of xml element in xml map |

### Examples

```csharp
// Called: cells.LinkToXmlMap("Transmittals_Map", 6, 12, "/Transmittals/Issued_Document");
public void Cells_Method_LinkToXmlMap()
{
    Workbook wb = new Workbook(SrcPath + "AddXmlMapping.xlsx");
    Worksheet sheet = wb.Worksheets["NotMerge"];
    Cells cells = sheet.Cells;

    cells.LinkToXmlMap("Transmittals_Map", 6, 5, "/Transmittals/Transmittal_folder/Element/Level");
    cells.LinkToXmlMap("Transmittals_Map", 6, 12, "/Transmittals/Issued_Document");

    Assert.AreEqual(sheet.ListObjects.Count, 3);

    ListObject table = sheet.ListObjects["Table811"];
    Assert.AreEqual(cells["M7"].StringValue, "Type");
    Assert.AreEqual(cells["N7"].StringValue, "Create_Date");
    Assert.AreEqual(cells["O7"].StringValue, "Create_User");
    Assert.AreEqual(table.StartColumn, 6);
    Assert.AreEqual(table.EndColumn, 11);

    wb.Save(Constants.destPath + "testAddXmlMappingNotMerge.xlsx");
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


