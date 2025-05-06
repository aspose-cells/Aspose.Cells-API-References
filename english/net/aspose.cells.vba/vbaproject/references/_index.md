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
// Called: vp.References.AddRegisteredReference(&amp;quot;stdole&amp;quot;, &amp;quot;*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation&amp;quot;);
[Test]
        public void Property_References()
        {
            Workbook workbook = new Workbook();
            VbaProject vp = workbook.VbaProject;
            vp.References.AddRegisteredReference(&quot;stdole&quot;, &quot;*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation&quot;);
            workbook.Save(Constants.destPath + &quot;CellsNet43925.xlsm&quot;);
        }
```

### See Also

* class [VbaProjectReferenceCollection](../../vbaprojectreferencecollection/)
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


