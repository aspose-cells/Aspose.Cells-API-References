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
            Workbook wb = new Workbook(Constants.sourcePath + "CELLSNET56699_56700.xlsx");
            OdsSaveOptions saveOptions = new OdsSaveOptions();
            saveOptions.OdfStrictVersion = Aspose.Cells.Ods.OpenDocumentFormatVersionType.Odf13;
            wb.Save(Constants.destPath + "CELLSNET56699_56700.ods", saveOptions);
            Assert.IsTrue(ManualFileUtil.ManualCheckStringInZip(Constants.destPath + "CELLSNET56699_56700.ods", "styles.xml", new string[] { "PageStyle_x_y_" }, true));
            Assert.IsTrue(ManualFileUtil.ManualCheckStringInZip(Constants.destPath + "CELLSNET56699_56700.ods", "content.xml", new string[] { "office:value=#" }, false));
        }
```

### See Also

* enum [OpenDocumentFormatVersionType](../../../aspose.cells.ods/opendocumentformatversiontype/)
* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


