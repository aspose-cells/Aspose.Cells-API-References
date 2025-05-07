---
title: VbaProject.Name
second_title: Aspose.Cells for .NET API Reference
description: VbaProject property. Gets and sets the name of the VBA project
type: docs
url: /net/aspose.cells.vba/vbaproject/name/
---
## VbaProject.Name property

Gets and sets the name of the VBA project.

```csharp
public string Name { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.VbaProject.Name, "VBAProject");
[Test]
        public void Property_Name()
        {
            Workbook workbook = new Workbook();
            Assert.AreEqual(workbook.VbaProject.Name, "VBAProject");
            workbook.Save(Constants.destPath + "CellsNet40353.xlsx");
        }
```

### See Also

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


