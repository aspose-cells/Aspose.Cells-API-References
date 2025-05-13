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
// Called: vbaProject.References.AddControlRefrernce("MSForms", "*\\G{0D452EE1-E08F-101A-852E-02608C4D0BB4}#2.0#0#C:\\Windows\\system32\\FM20.DLL#Microsoft Forms 2.0 Object Library", "twiddledLibid", "extendedLibid");
public static void VbaProjectReferenceCollection_Method_AddControlRefrernce()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();
            
            // Init VBA project
            VbaProject vbaProject = workbook.VbaProject;
            
            // Add VBA project reference
            vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
            
            // Add another VBA project reference
            vbaProject.References.AddControlRefrernce("MSForms", "*\\G{0D452EE1-E08F-101A-852E-02608C4D0BB4}#2.0#0#C:\\Windows\\system32\\FM20.DLL#Microsoft Forms 2.0 Object Library", "twiddledLibid", "extendedLibid");
            
            // Add project reference
            vbaProject.References.AddProjectRefrernce("MyProject", "absoluteLibid", "relativeLibid");
            
            // Accessing the references collection
            VbaProjectReferenceCollection references = vbaProject.References;
            
            // Displaying the count of references
            Console.WriteLine("Total References: " + references.Count);
            
            // Accessing a specific reference
            VbaProjectReference reference = references[0];
            Console.WriteLine("First Reference Name: " + reference.Name);
            
            // Copying references from another collection (assuming anotherVbaProjectReferences is another VbaProjectReferenceCollection)
            // VbaProjectReferenceCollection anotherVbaProjectReferences = ...;
            // references.Copy(anotherVbaProjectReferences);
            
            // Saving the Excel file
            workbook.Save("VbaProjectReferenceCollectionExample.xlsm");
        }
```

### See Also

* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


