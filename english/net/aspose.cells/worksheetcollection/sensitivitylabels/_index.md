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
// Called: Assert.AreEqual(&amp;quot;{7e848398-70bd-400c-b8cf-2ab6f30d1b60}&amp;quot;, workbook.Worksheets.SensitivityLabels[0].SiteId);
[Test]
        public void Property_SensitivityLabels()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Net56491.xlsx&quot;);
            MemoryStream ms = Util.SaveAsBuffer(workbook, SaveFormat.Xlsx);
            Assert.IsFalse(ManualFileUtil.ManualCheckStringInZip(ms,
            //workbook.Save(Constants.destPath + &quot;Net56491.xlsx&quot;);
            //Assert.IsFalse(ManualFileUtil.ManualCheckStringInZip(Constants.destPath + &quot;Net56491.xlsx&quot;,
                &quot;docMetadata/LabelInfo.xml&quot;, new string[] { &quot;&lt;clbl:label&quot; }, false));
            Assert.AreEqual(&quot;{7e848398-70bd-400c-b8cf-2ab6f30d1b60}&quot;, workbook.Worksheets.SensitivityLabels[0].SiteId);
        }
```

### See Also

* class [SensitivityLabelCollection](../../../aspose.cells.metas/sensitivitylabelcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


