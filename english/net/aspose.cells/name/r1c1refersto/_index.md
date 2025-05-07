---
title: Name.R1C1RefersTo
second_title: Aspose.Cells for .NET API Reference
description: Name property. Gets or sets a R1C1 reference of the Name
type: docs
url: /net/aspose.cells/name/r1c1refersto/
---
## Name.R1C1RefersTo property

Gets or sets a R1C1 reference of the [`Name`](../).

```csharp
public string R1C1RefersTo { get; set; }
```

### Examples

```csharp
// Called: name.R1C1RefersTo = ("'Allo''wed'!R3C1:R9C4");
[Test]
        public void Property_R1C1RefersTo()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSJAVA41042.xlsx");
            int rangeIndex = workbook.Worksheets.Names.Add("dummyrange");
            Name name = workbook.Worksheets.Names[rangeIndex];

            name.R1C1RefersTo = ("'Allo''wed'!R3C1:R9C4");
            name = workbook.Worksheets.Names[rangeIndex];
            Assert.AreEqual(name.RefersTo.StartsWith("="), true);
        }
```

### See Also

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


