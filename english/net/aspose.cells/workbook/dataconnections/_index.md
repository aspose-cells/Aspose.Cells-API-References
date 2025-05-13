---
title: Workbook.DataConnections
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Gets the ExternalConnection collection
type: docs
url: /net/aspose.cells/workbook/dataconnections/
---
## Workbook.DataConnections property

Gets the [`ExternalConnection`](../../../aspose.cells.externalconnections/externalconnection/) collection.

```csharp
public ExternalConnectionCollection DataConnections { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(1,n.DataConnections.Count);
public void Workbook_Property_DataConnections()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Workbook n = new Workbook();
    //int i = 0;
    foreach (Worksheet sheet in workbook.Worksheets)
    {
        Worksheet s = n.Worksheets.Add(sheet.Name);
        //s.Copy(sheet);

    }
    foreach (Worksheet sheet in workbook.Worksheets)
    {
        Worksheet s = n.Worksheets[sheet.Name];
        CopyOptions copyOptions = new CopyOptions();
        copyOptions.ReferToSheetWithSameName = true;
        s.Copy(sheet, copyOptions);
    }
    Assert.AreEqual(1,n.DataConnections.Count);
    Util.ReSave(n, SaveFormat.Xlsx);
    //n.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [ExternalConnectionCollection](../../../aspose.cells.externalconnections/externalconnectioncollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


