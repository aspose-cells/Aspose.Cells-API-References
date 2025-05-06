---
title: VbaProjectReference.Type
second_title: Aspose.Cells for .NET API Reference
description: VbaProjectReference property. Gets the type of this reference
type: docs
url: /net/aspose.cells.vba/vbaprojectreference/type/
---
## VbaProjectReference.Type property

Gets the type of this reference.

```csharp
public VbaProjectReferenceType Type { get; }
```

### Examples

```csharp
// Called: switch (x.Type.ToString())
[Test]
        public void Property_Type()
        {
            var targetwb = new Workbook();
            var sourcewb = new Workbook(Constants.sourcePath + @&quot;CellsNet47599.xlsm&quot;);
            targetwb.VbaProject.References.Clear();
            foreach (VbaProjectReference x in sourcewb.VbaProject.References)
            {
                switch (x.Type.ToString())
                {
                    case &quot;Registered&quot;:
                        targetwb.VbaProject.References.AddRegisteredReference(x.Name, x.Libid);
                        break;

                    case &quot;Control&quot;:
                        targetwb.VbaProject.References.AddControlRefrernce(x.Name, x.Libid, x.Twiddledlibid, x.ExtendedLibid);

                        break;
                    default: break;
                }

            }
            Assert.AreEqual(4, targetwb.VbaProject.References.Count);
            targetwb.Save(Constants.destPath + &quot;CellsNet47599.xlsm&quot;);

        }
```

### See Also

* enum [VbaProjectReferenceType](../../vbaprojectreferencetype/)
* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


