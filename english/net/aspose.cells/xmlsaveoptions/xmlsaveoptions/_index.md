---
title: XmlSaveOptions.XmlSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: XmlSaveOptions constructor. Creates options for saving xml file
type: docs
url: /net/aspose.cells/xmlsaveoptions/xmlsaveoptions/
---
## XmlSaveOptions constructor

Creates options for saving xml file.

```csharp
public XmlSaveOptions()
```

### Examples

```csharp
// Called: saveOptions = new XmlSaveOptions();
[Test]
        public void XmlSaveOptions_Constructor()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet53135.xlsx&quot;);
            XmlSaveOptions saveOptions = new XmlSaveOptions();
            saveOptions.SheetNameAsElementName = true;
            workbook.Save(Constants.destPath + &quot;CellsNet53135_1.xml&quot;, saveOptions);
            string text = File.ReadAllText(Constants.destPath + &quot;CellsNet53135_1.xml&quot;);
            Assert.IsTrue(text.IndexOf(&quot;&lt;c&gt;63&lt;/c&gt;&quot;) != -1);

            saveOptions = new XmlSaveOptions();
            saveOptions.SheetNameAsElementName = true;
            saveOptions.DataAsAttribute = true;
            workbook.Save(Constants.destPath + &quot;CellsNet53135_2.xml&quot;, saveOptions);
            text = File.ReadAllText(Constants.destPath + &quot;CellsNet53135_2.xml&quot;);

            Assert.IsTrue(text.IndexOf(&quot;c=\&quot;63\&quot;&quot;) != -1);

        }
```

### See Also

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


