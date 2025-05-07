---
title: VbaProject.Protect
second_title: Aspose.Cells for .NET API Reference
description: VbaProject method. Protects or unprotects this VBA project
type: docs
url: /net/aspose.cells.vba/vbaproject/protect/
---
## VbaProject.Protect method

Protects or unprotects this VBA project.

```csharp
public void Protect(bool islockedForViewing, string password)
```

| Parameter | Type | Description |
| --- | --- | --- |
| islockedForViewing | Boolean | indicates whether locks project for viewing. |
| password | String | If the value is null, unprotects this VBA project, otherwise projects the this VBA project. |

### Remarks

If islockedForViewing is true, the password could not be null.

### Examples

```csharp
// Called: workbook.VbaProject.Protect(false, null);
[Test]
        public void Method_String_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET46464.xlsm");
            workbook.VbaProject.Protect(false, null);
            Util.SaveForViewer(workbook, "13", "CELLSNET46464.xlsm");
        }
```

### See Also

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


