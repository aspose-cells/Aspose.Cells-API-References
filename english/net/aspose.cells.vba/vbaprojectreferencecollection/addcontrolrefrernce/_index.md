---
title: VbaProjectReferenceCollection.AddControlRefrernce
second_title: Aspose.Cells for .NET API Reference
description: VbaProjectReferenceCollection method. Add a reference to a twiddled type library and its extended type library
type: docs
url: /net/aspose.cells.vba/vbaprojectreferencecollection/addcontrolrefrernce/
---
## VbaProjectReferenceCollection.AddControlRefrernce method

Add a reference to a twiddled type library and its extended type library.

```csharp
public int AddControlRefrernce(string name, string libid, string twiddledlibid, 
    string extendedLibid)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of reference. |
| libid | String | The identifier of an Automation type library. |
| twiddledlibid | String | The identifier of a twiddled type library |
| extendedLibid | String | The identifier of an extended type library |

### Examples

```csharp
// Called: targetwb.VbaProject.References.AddControlRefrernce(x.Name, x.Libid, x.Twiddledlibid, x.ExtendedLibid);
[Test]
        public void Method_String_()
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

* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


