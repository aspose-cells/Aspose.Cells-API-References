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
// Called: wb.RibbonXml = sr.ReadToEnd();
[Test]
        public void Property_RibbonXml()
        {
            Workbook wb = new Workbook(Constants.openPivottablePath + "40423.xlsx");
            FileInfo fi = new FileInfo(Constants.openPivottablePath + "customUI.xml");
            StreamReader sr = fi.OpenText();
            wb.RibbonXml = sr.ReadToEnd();
            sr.Close();
            wb.Save(Constants.savePivottablePath + "40423.xlsx");
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


