---
title: VbaProjectReference.Libid
second_title: Aspose.Cells for .NET API Reference
description: VbaProjectReference property. Gets and sets the Libid of the reference
type: docs
url: /net/aspose.cells.vba/vbaprojectreference/libid/
---
## VbaProjectReference.Libid property

Gets and sets the Libid of the reference.

```csharp
public string Libid { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine(&amp;quot;Reference Libid: &amp;quot; + reference.Libid);
public static void Property_Libid()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();

            // Init VBA project
            VbaProject vbaProject = workbook.VbaProject;

            // Add VBA project reference
            vbaProject.References.AddRegisteredReference(&quot;stdole&quot;, &quot;*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation&quot;);

            // Saving the Excel file
            workbook.Save(&quot;VbaProjectReferenceTypeExample.xlsm&quot;);

            // Demonstrating the use of VbaProjectReferenceType enum
            VbaProjectReference reference = vbaProject.References[0];
            Console.WriteLine(&quot;Reference Type: &quot; + reference.Type);
            Console.WriteLine(&quot;Reference Name: &quot; + reference.Name);
            Console.WriteLine(&quot;Reference Libid: &quot; + reference.Libid);
        }
```

### See Also

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


