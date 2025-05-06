---
title: VbaProject.Encoding
second_title: Aspose.Cells for .NET API Reference
description: VbaProject property. Gets and sets the encoding of VBA project
type: docs
url: /net/aspose.cells.vba/vbaproject/encoding/
---
## VbaProject.Encoding property

Gets and sets the encoding of VBA project.

```csharp
public Encoding Encoding { get; set; }
```

### Examples

```csharp
// Called: vbaProject.Encoding = Encoding.UTF8;
public static void Property_Encoding()
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

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


