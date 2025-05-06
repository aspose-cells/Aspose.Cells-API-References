---
title: VbaProjectReferenceCollection.AddProjectRefrernce
second_title: Aspose.Cells for .NET API Reference
description: VbaProjectReferenceCollection method. Adds a reference to an external VBA project
type: docs
url: /net/aspose.cells.vba/vbaprojectreferencecollection/addprojectrefrernce/
---
## VbaProjectReferenceCollection.AddProjectRefrernce method

Adds a reference to an external VBA project.

```csharp
public int AddProjectRefrernce(string name, string absoluteLibid, string relativeLibid)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of reference. |
| absoluteLibid | String | The referenced VBA project's identifier with an absolute path. |
| relativeLibid | String | The referenced VBA project's identifier with an relative path. |

### Examples

```csharp
// Called: refs.AddProjectRefrernce(name, @&amp;quot;*\C&amp;quot; + referencePath, @&amp;quot;*\C&amp;quot; + referencePath);
[Test]
        public void Method_String_()
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

* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


