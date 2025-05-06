---
title: VbaProjectReferenceCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: VbaProjectReferenceCollection property. Get the reference in the list by the index
type: docs
url: /net/aspose.cells.vba/vbaprojectreferencecollection/item/
---
## VbaProjectReferenceCollection indexer

Get the reference in the list by the index.

```csharp
public VbaProjectReference this[int i] { get; }
```

| Parameter | Description |
| --- | --- |
| i | The index. |

### Examples

```csharp
// Called: VbaProjectReference reference = references[0];
public static void Property_Int32_()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();
            
            // Init VBA project
            VbaProject vbaProject = workbook.VbaProject;
            
            // Add VBA project reference
            vbaProject.References.AddRegisteredReference(&quot;stdole&quot;, &quot;*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation&quot;);
            
            // Add another VBA project reference
            vbaProject.References.AddControlRefrernce(&quot;MSForms&quot;, &quot;*\\G{0D452EE1-E08F-101A-852E-02608C4D0BB4}#2.0#0#C:\\Windows\\system32\\FM20.DLL#Microsoft Forms 2.0 Object Library&quot;, &quot;twiddledLibid&quot;, &quot;extendedLibid&quot;);
            
            // Add project reference
            vbaProject.References.AddProjectRefrernce(&quot;MyProject&quot;, &quot;absoluteLibid&quot;, &quot;relativeLibid&quot;);
            
            // Accessing the references collection
            VbaProjectReferenceCollection references = vbaProject.References;
            
            // Displaying the count of references
            Console.WriteLine(&quot;Total References: &quot; + references.Count);
            
            // Accessing a specific reference
            VbaProjectReference reference = references[0];
            Console.WriteLine(&quot;First Reference Name: &quot; + reference.Name);
            
            // Copying references from another collection (assuming anotherVbaProjectReferences is another VbaProjectReferenceCollection)
            // VbaProjectReferenceCollection anotherVbaProjectReferences = ...;
            // references.Copy(anotherVbaProjectReferences);
            
            // Saving the Excel file
            workbook.Save(&quot;VbaProjectReferenceCollectionExample.xlsm&quot;);
        }
```

### See Also

* class [VbaProjectReference](../../vbaprojectreference/)
* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


