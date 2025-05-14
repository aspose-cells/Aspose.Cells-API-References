---
title: VbaProjectReference.ExtendedLibid
second_title: Aspose.Cells for .NET API Reference
description: VbaProjectReference property. Gets and sets the extended Libid of the reference
type: docs
url: /net/aspose.cells.vba/vbaprojectreference/extendedlibid/
---
## VbaProjectReference.ExtendedLibid property

Gets and sets the extended Libid of the reference.

```csharp
public string ExtendedLibid { get; set; }
```

### Remarks

Only for control reference.

### Examples

```csharp
// Called: targetwb.VbaProject.References.AddControlRefrernce(x.Name, x.Libid, x.Twiddledlibid, x.ExtendedLibid);
public void VbaProjectReference_Property_ExtendedLibid()
{
    var targetwb = new Workbook();
    var sourcewb = new Workbook(Constants.sourcePath + @"example.xlsm");
    targetwb.VbaProject.References.Clear();
    foreach (VbaProjectReference x in sourcewb.VbaProject.References)
    {
        switch (x.Type.ToString())
        {
            case "Registered":
                targetwb.VbaProject.References.AddRegisteredReference(x.Name, x.Libid);
                break;

            case "Control":
                targetwb.VbaProject.References.AddControlRefrernce(x.Name, x.Libid, x.Twiddledlibid, x.ExtendedLibid);

                break;
            default: break;
        }

    }
    Assert.AreEqual(4, targetwb.VbaProject.References.Count);
    targetwb.Save(Constants.destPath + "example.xlsm");

}
```

### See Also

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


