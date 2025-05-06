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
            string path = Constants.sourcePath + &quot;Vba/&quot;;
            Workbook wb = new Workbook(path + &quot;load.xlsm&quot;);
            VbaProject vbaProject = wb.VbaProject;
            Assert.IsFalse(vbaProject.IsProtected);
            Assert.IsFalse(vbaProject.IslockedForViewing);

            wb = new Workbook(path + &quot;load_protected.xlsm&quot;);
            vbaProject = wb.VbaProject;
            Assert.IsTrue(vbaProject.IsProtected);
            Assert.IsFalse(vbaProject.IslockedForViewing);

            wb = new Workbook(path + &quot;load_protected_lockedForView.xlsm&quot;);
            vbaProject = wb.VbaProject;
            Assert.IsTrue(vbaProject.IsProtected);
            Assert.IsTrue(vbaProject.IslockedForViewing);
        }
```

### See Also

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


