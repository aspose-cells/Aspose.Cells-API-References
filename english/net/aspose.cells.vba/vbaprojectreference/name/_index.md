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
            Workbook workBook = new Workbook(Constants.sourcePath + "CellsNet44600.xlsm");
            VbaProjectReferenceCollection refs = workBook.VbaProject.References;

            string name = "ExternalMakroProject";
            string referencePath = @"\\BABARRAZA-PC\Users\Babar Raza\Downloads\shared-folder\ExcelMakros.xla";

            int foundReferenceIndex = -1;

            for (int i = 0; i < refs.Count; i++)
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
            refs.AddProjectRefrernce(name, @"*\C" + referencePath, @"*\C" + referencePath);
            workBook.Save(Constants.destPath + "CellsNet44600.xlsm");
            workBook.Save(Constants.destPath + "CellsNet44600.xlsm"); //<- Exception occurs 
        }
```

### See Also

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


