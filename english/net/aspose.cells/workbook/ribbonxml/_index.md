---
title: Workbook.RibbonXml
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Gets and sets the XML file that defines the Ribbon UI
type: docs
url: /net/aspose.cells/workbook/ribbonxml/
---
## Workbook.RibbonXml property

Gets and sets the XML file that defines the Ribbon UI.

```csharp
public string RibbonXml { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(workbook.RibbonXml != null);
public void Workbook_Property_RibbonXml()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsm");
    Assert.IsTrue(workbook.RibbonXml != null);
    workbook.Save(Constants.destPath + "example.xlsm");
    workbook = new Workbook(Constants.destPath + "example.xlsm");
    Assert.IsTrue(workbook.RibbonXml != null);
}
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


