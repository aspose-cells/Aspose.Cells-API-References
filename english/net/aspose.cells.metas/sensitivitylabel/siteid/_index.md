---
title: SensitivityLabel.SiteId
second_title: Aspose.Cells for .NET API Reference
description: SensitivityLabel property. Represents the Azure Active Directory Azure AD site identifier corresponding to the sensitivity label policy which describes the sensitivity label
type: docs
url: /net/aspose.cells.metas/sensitivitylabel/siteid/
---
## SensitivityLabel.SiteId property

Represents the Azure Active Directory (Azure AD) site identifier corresponding to the sensitivity label policy which describes the sensitivity label.

```csharp
public string SiteId { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual("{7e848398-70bd-400c-b8cf-2ab6f30d1b60}", workbook.Worksheets.SensitivityLabels[0].SiteId);
[Test]
        public void Property_SiteId()
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

* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


