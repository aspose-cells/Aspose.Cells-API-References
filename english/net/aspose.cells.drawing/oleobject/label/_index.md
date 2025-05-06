---
title: OleObject.Label
second_title: Aspose.Cells for .NET API Reference
description: OleObject property. Gets and sets the display label of the linked ole object
type: docs
url: /net/aspose.cells.drawing/oleobject/label/
---
## OleObject.Label property

Gets and sets the display label of the linked ole object.

```csharp
public string Label { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(oleObject.Label, &amp;quot;label_nameです&amp;quot;);
[Test]
        public void Property_Label()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSJAVA42543.xlsx&quot;);
            OleObject oleObject = workbook.Worksheets[0].OleObjects[0];
            Assert.AreEqual(oleObject.Label, &quot;label_nameです&quot;);
            workbook.Save(Constants.destPath + &quot;CELLSJAVA42543.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSJAVA42543.xlsx&quot;);
            oleObject = workbook.Worksheets[0].OleObjects[0];
            Assert.AreEqual(oleObject.Label, &quot;label_nameです&quot;);
        }
```

### See Also

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


