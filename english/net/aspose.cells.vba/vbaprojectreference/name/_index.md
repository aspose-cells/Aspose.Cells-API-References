---
title: VbaProjectReference.Name
second_title: Aspose.Cells for .NET API Reference
description: VbaProjectReference property. Gets and sets the name of the reference
type: docs
url: /net/aspose.cells.vba/vbaprojectreference/name/
---
## VbaProjectReference.Name property

Gets and sets the name of the reference.

```csharp
public string Name { get; set; }
```

### Examples

```csharp
// Called: if (refs[i].Name.Equals(name))
[Test]
        public void Property_Name()
        {
            Workbook workBook = new Workbook(Constants.sourcePath + &quot;CellsNet44600.xlsm&quot;);
            VbaProjectReferenceCollection refs = workBook.VbaProject.References;

            string name = &quot;ExternalMakroProject&quot;;
            string referencePath = @&quot;\\BABARRAZA-PC\Users\Babar Raza\Downloads\shared-folder\ExcelMakros.xla&quot;;

            int foundReferenceIndex = -1;

            for (int i = 0; i &lt; refs.Count; i++)
            {
                if (refs[i].Name.Equals(name))
                {
                    foundReferenceIndex = i;
                    break;
                }
            }

            if (foundReferenceIndex != -1)
            {
                refs.RemoveAt(foundReferenceIndex);
            }
            refs.AddProjectRefrernce(name, @&quot;*\C&quot; + referencePath, @&quot;*\C&quot; + referencePath);
            workBook.Save(Constants.destPath + &quot;CellsNet44600.xlsm&quot;);
            workBook.Save(Constants.destPath + &quot;CellsNet44600.xlsm&quot;); //&lt;- Exception occurs 
        }
```

### See Also

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


