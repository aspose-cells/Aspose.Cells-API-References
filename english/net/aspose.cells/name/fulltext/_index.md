---
title: Name.FullText
second_title: Aspose.Cells for .NET API Reference
description: Name property. Gets the name full text of the object with the scope setting
type: docs
url: /net/aspose.cells/name/fulltext/
---
## Name.FullText property

Gets the name full text of the object with the scope setting.

```csharp
public string FullText { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual("'Q''re'!TestName", nc[0].FullText);
[Test]
        public void Property_FullText()
        {
            Workbook wb = new Workbook();
            wb.Worksheets.Add("Q're");
            NameCollection nc = wb.Worksheets.Names;
            nc[nc.Add("'Q''re'!TestName")].RefersTo = "='Q''re'!$A$1";
            Assert.AreEqual("'Q''re'!TestName", nc[0].FullText);
            Assert.AreEqual("='Q''re'!$A$1", nc[0].RefersTo);
        }
```

### See Also

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


