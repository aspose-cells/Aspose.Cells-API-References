---
title: WorksheetCollection.SensitivityLabels
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection property. Represents all sensitivity labels
type: docs
url: /net/aspose.cells/worksheetcollection/sensitivitylabels/
---
## WorksheetCollection.SensitivityLabels property

Represents all sensitivity labels.

```csharp
public SensitivityLabelCollection SensitivityLabels { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual("{7e848398-70bd-400c-b8cf-2ab6f30d1b60}", workbook.Worksheets.SensitivityLabels[0].SiteId);
[Test]
        public void Property_SensitivityLabels()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "Net56491.xlsx");
            MemoryStream ms = Util.SaveAsBuffer(workbook, SaveFormat.Xlsx);
            Assert.IsFalse(ManualFileUtil.ManualCheckStringInZip(ms,
            //workbook.Save(Constants.destPath + "Net56491.xlsx");
            //Assert.IsFalse(ManualFileUtil.ManualCheckStringInZip(Constants.destPath + "Net56491.xlsx",
                "docMetadata/LabelInfo.xml", new string[] { "<clbl:label" }, false));
            Assert.AreEqual("{7e848398-70bd-400c-b8cf-2ab6f30d1b60}", workbook.Worksheets.SensitivityLabels[0].SiteId);
        }
```

### See Also

* class [SensitivityLabelCollection](../../../aspose.cells.metas/sensitivitylabelcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


