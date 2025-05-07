---
title: VbaProjectReference.Twiddledlibid
second_title: Aspose.Cells for .NET API Reference
description: VbaProjectReference property. Gets and sets the twiddled Libid of the reference
type: docs
url: /net/aspose.cells.vba/vbaprojectreference/twiddledlibid/
---
## VbaProjectReference.Twiddledlibid property

Gets and sets the twiddled Libid of the reference.

```csharp
public string Twiddledlibid { get; set; }
```

### Remarks

Only for control reference.

### Examples

```csharp
// Called: targetwb.VbaProject.References.AddControlRefrernce(x.Name, x.Libid, x.Twiddledlibid, x.ExtendedLibid);
[Test]
        public void Property_Twiddledlibid()
        {
            var targetwb = new Workbook();
            var sourcewb = new Workbook(Constants.sourcePath + @"CellsNet47599.xlsm");
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
            targetwb.Save(Constants.destPath + "CellsNet47599.xlsm");

        }
```

### See Also

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


