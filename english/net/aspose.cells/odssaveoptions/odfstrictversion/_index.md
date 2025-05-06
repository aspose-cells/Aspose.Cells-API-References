---
title: OdsSaveOptions.OdfStrictVersion
second_title: Aspose.Cells for .NET API Reference
description: OdsSaveOptions property. Gets and sets the ODF version
type: docs
url: /net/aspose.cells/odssaveoptions/odfstrictversion/
---
## OdsSaveOptions.OdfStrictVersion property

Gets and sets the ODF version.

```csharp
public OpenDocumentFormatVersionType OdfStrictVersion { get; set; }
```

### Examples

```csharp
// Called: saveOptions.OdfStrictVersion = Aspose.Cells.Ods.OpenDocumentFormatVersionType.Odf13;
[Test]
        public void Property_OdfStrictVersion()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSNET56699_56700.xlsx&quot;);
            OdsSaveOptions saveOptions = new OdsSaveOptions();
            saveOptions.OdfStrictVersion = Aspose.Cells.Ods.OpenDocumentFormatVersionType.Odf13;
            wb.Save(Constants.destPath + &quot;CELLSNET56699_56700.ods&quot;, saveOptions);
            Assert.IsTrue(ManualFileUtil.ManualCheckStringInZip(Constants.destPath + &quot;CELLSNET56699_56700.ods&quot;, &quot;styles.xml&quot;, new string[] { &quot;PageStyle_x_y_&quot; }, true));
            Assert.IsTrue(ManualFileUtil.ManualCheckStringInZip(Constants.destPath + &quot;CELLSNET56699_56700.ods&quot;, &quot;content.xml&quot;, new string[] { &quot;office:value=#&quot; }, false));
        }
```

### See Also

* enum [OpenDocumentFormatVersionType](../../../aspose.cells.ods/opendocumentformatversiontype/)
* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


