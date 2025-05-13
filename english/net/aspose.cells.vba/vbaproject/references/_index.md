---
title: VbaProject.References
second_title: Aspose.Cells for .NET API Reference
description: VbaProject property. Gets all references of VBA project
type: docs
url: /net/aspose.cells.vba/vbaproject/references/
---
## VbaProject.References property

Gets all references of VBA project.

```csharp
public VbaProjectReferenceCollection References { get; }
```

### Examples

```csharp
// Called: targetwb.VbaProject.References.Clear();
public void VbaProject_Property_References()
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

* class [VbaProjectReferenceCollection](../../vbaprojectreferencecollection/)
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


