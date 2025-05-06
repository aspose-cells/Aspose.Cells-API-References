---
title: Workbook.CustomXmlParts
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Represents a Custom XML Data Storage Part custom XML data within a package
type: docs
url: /net/aspose.cells/workbook/customxmlparts/
---
## Workbook.CustomXmlParts property

Represents a Custom XML Data Storage Part (custom XML data within a package).

```csharp
public CustomXmlPartCollection CustomXmlParts { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(3, workboook.CustomXmlParts.Count);
[Test]
        public void Property_CustomXmlParts()
        {
            Workbook workboook = new Workbook(Constants.sourcePath + &quot;CELLSNET44472.xls&quot;);
            Assert.AreEqual(3, workboook.CustomXmlParts.Count);
            workboook.CustomXmlParts.Clear();
            workboook.Save(Constants.destPath + &quot;CELLSNET44472.xls&quot;);
            workboook = new Workbook(Constants.destPath + &quot;CELLSNET44472.xls&quot;);
            Assert.AreEqual(0, workboook.CustomXmlParts.Count);
        }
```

### See Also

* class [CustomXmlPartCollection](../../../aspose.cells.markup/customxmlpartcollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


