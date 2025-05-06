---
title: XmlLoadOptions.XmlLoadOptions
second_title: Aspose.Cells for .NET API Reference
description: XmlLoadOptions constructor. Represents the options of loading xml file
type: docs
url: /net/aspose.cells/xmlloadoptions/xmlloadoptions/
---
## XmlLoadOptions() {#constructor}

Represents the options of loading xml file.

```csharp
public XmlLoadOptions()
```

### Examples

```csharp
// Called: XmlLoadOptions loadOptions = new XmlLoadOptions();
[Test]
        public void XmlLoadOptions_Constructor()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET49717.xlsx&quot;);
            XmlSaveOptions saveOptions = new XmlSaveOptions();
            saveOptions.SheetNameAsElementName = false;
            workbook.Save(Constants.destPath + &quot;CELLSNET49717.xml&quot;, saveOptions);
            XmlLoadOptions loadOptions = new XmlLoadOptions();
            loadOptions.ContainsMultipleWorksheets = true;
            workbook = new Workbook(Constants.destPath + &quot;CELLSNET49717.xml&quot;, loadOptions);
            workbook.Save(Constants.destPath + &quot;CELLSNET49717.xlsx&quot;);
            Assert.AreEqual(&quot;Firstname&quot;, workbook.Worksheets[0].Cells[&quot;C3&quot;].StringValue);
            
        }
```

### See Also

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## XmlLoadOptions(LoadFormat) {#constructor_1}

Represents the options of loading xml file.

```csharp
public XmlLoadOptions(LoadFormat type)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | LoadFormat | The load format type. |

### See Also

* enum [LoadFormat](../../loadformat/)
* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


