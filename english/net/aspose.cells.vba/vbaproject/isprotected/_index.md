---
title: VbaProject.IsProtected
second_title: Aspose.Cells for .NET API Reference
description: VbaProject property. Indicates whether this VBA project is protected
type: docs
url: /net/aspose.cells.vba/vbaproject/isprotected/
---
## VbaProject.IsProtected property

Indicates whether this VBA project is protected.

```csharp
public bool IsProtected { get; }
```

### Examples

```csharp
// Called: Assert.IsFalse(vbaProject.IsProtected);
[Test]
        public void Property_IsProtected()
        {
            string path = Constants.sourcePath + "Vba/";
            Workbook wb = new Workbook(path + "load.xlsm");
            VbaProject vbaProject = wb.VbaProject;
            Assert.IsFalse(vbaProject.IsProtected);
            Assert.IsFalse(vbaProject.IslockedForViewing);

            wb = new Workbook(path + "load_protected.xlsm");
            vbaProject = wb.VbaProject;
            Assert.IsTrue(vbaProject.IsProtected);
            Assert.IsFalse(vbaProject.IslockedForViewing);

            wb = new Workbook(path + "load_protected_lockedForView.xlsm");
            vbaProject = wb.VbaProject;
            Assert.IsTrue(vbaProject.IsProtected);
            Assert.IsTrue(vbaProject.IslockedForViewing);
        }
```

### See Also

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


