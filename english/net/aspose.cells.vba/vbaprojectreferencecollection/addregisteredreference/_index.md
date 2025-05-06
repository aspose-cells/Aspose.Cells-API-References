---
title: VbaProjectReferenceCollection.AddRegisteredReference
second_title: Aspose.Cells for .NET API Reference
description: VbaProjectReferenceCollection method. Add a reference to an Automation type library
type: docs
url: /net/aspose.cells.vba/vbaprojectreferencecollection/addregisteredreference/
---
## VbaProjectReferenceCollection.AddRegisteredReference method

Add a reference to an Automation type library.

```csharp
public int AddRegisteredReference(string name, string libid)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of reference. |
| libid | String | The identifier of an Automation type library. |

### Examples

```csharp
// Called: vbaProject.References.AddRegisteredReference(&amp;quot;stdole&amp;quot;, &amp;quot;*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation&amp;quot;);
public static void Method_String_()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();

            // Init VBA project
            VbaProject vbaProject = workbook.VbaProject;

            // Setting properties
            vbaProject.Name = &quot;MyVbaProject&quot;;
            vbaProject.Encoding = Encoding.UTF8;

            // Checking read-only properties
            bool isSigned = vbaProject.IsSigned;
            bool isProtected = vbaProject.IsProtected;
            bool isLockedForViewing = vbaProject.IslockedForViewing;
            bool isValidSigned = vbaProject.IsValidSigned;

            // Adding a VBA module
            int moduleIndex = vbaProject.Modules.Add(VbaModuleType.Class, &quot;MyModule&quot;);

            // Adding a VBA project reference
            vbaProject.References.AddRegisteredReference(&quot;stdole&quot;, &quot;*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation&quot;);

            // Protecting the VBA project
            vbaProject.Protect(true, &quot;password&quot;);

            // Signing the VBA project
            X509Certificate2 certificate = new X509Certificate2(&quot;path_to_certificate.pfx&quot;, &quot;certificate_password&quot;);
            DigitalSignature digitalSignature = new DigitalSignature(certificate, &quot;Signature Comments&quot;, DateTime.Now);
            vbaProject.Sign(digitalSignature);

            // Saving the Excel file
            workbook.Save(&quot;VbaProjectExample.xlsm&quot;);

            return;
        }
```

### See Also

* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


