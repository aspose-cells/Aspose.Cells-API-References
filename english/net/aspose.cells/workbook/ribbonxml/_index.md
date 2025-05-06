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
           
            Workbook wb = new Workbook();

            var uiXML = Constants.sourcePath + &quot;CELLSNET51632_CustomUI.xml&quot;;

            FileInfo fi = new FileInfo(uiXML);

            StreamReader sr = fi.OpenText();

            wb.RibbonXml = sr.ReadToEnd();

            sr.Close();

            wb.Save(Constants.destPath + &quot;CELLSNET51632.xlsx&quot;);

            Assert.IsTrue(ManualFileUtil.ManualCheckStringInZip(Constants.destPath + &quot;CELLSNET51632.xlsx&quot;, 
                &quot;_rels/.rels&quot;, new string[] { &quot;http://schemas.microsoft.com/office/2007/relationships/ui/extensibility&quot; }, true));
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


