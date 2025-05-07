---
title: VbaProject.IslockedForViewing
second_title: Aspose.Cells for .NET API Reference
description: VbaProject property. Indicates whether this VBA project is locked for viewing
type: docs
url: /net/aspose.cells.vba/vbaproject/islockedforviewing/
---
## VbaProject.IslockedForViewing property

Indicates whether this VBA project is locked for viewing.

```csharp
public bool IslockedForViewing { get; }
```

### Examples

```csharp
// Called: Assert.IsFalse(vbaProject.IslockedForViewing);
[Test]
        public void Property_IslockedForViewing()
        {
            MemoryStream ms = new MemoryStream();
            string path = Constants.sourcePath + "Vba/";
            Workbook wb = new Workbook(path + "load.xlsm");
            VbaProject vbaProject = wb.VbaProject;

            //protect, lock for view
            vbaProject.Protect(true, "abc123");
            Assert.IsTrue(vbaProject.IsProtected);
            Assert.IsTrue(vbaProject.IslockedForViewing);
            wb.Save(ms, SaveFormat.Xlsm);
            wb = new Workbook(ms);
            vbaProject = wb.VbaProject;
            Assert.IsTrue(vbaProject.IsProtected);
            Assert.IsTrue(vbaProject.IslockedForViewing);

            //only protect
            vbaProject.Protect(false, "123456");
            Assert.IsTrue(vbaProject.IsProtected);
            Assert.IsFalse(vbaProject.IslockedForViewing);
            ms.SetLength(0);
            wb.Save(ms, SaveFormat.Xlsm);
            wb = new Workbook(ms);
            vbaProject = wb.VbaProject;
            Assert.IsTrue(vbaProject.IsProtected);
            Assert.IsFalse(vbaProject.IslockedForViewing);

            //clear protect
            vbaProject.Protect(true, "");
            Assert.IsFalse(vbaProject.IsProtected);
            Assert.IsFalse(vbaProject.IslockedForViewing);
            ms.SetLength(0);
            wb.Save(ms, SaveFormat.Xlsm);
            wb = new Workbook(ms);
            vbaProject = wb.VbaProject;
            Assert.IsFalse(vbaProject.IsProtected);
            Assert.IsFalse(vbaProject.IslockedForViewing);
        }
```

### See Also

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


