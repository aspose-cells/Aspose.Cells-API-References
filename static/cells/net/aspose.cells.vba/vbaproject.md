##Class VbaProject
Aspose.Cells.Vba.VbaProject class. Represents the VBA project
## VbaProject class
Represents the VBA project.
```csharp
public class VbaProject
```
## Properties
| Name | Description |
| --- | --- |
| [CertRawData](../../aspose.cells.vba/vbaproject/certrawdata/) { get; } | Gets certificate raw data if this VBA project is signed. |
| [Encoding](../../aspose.cells.vba/vbaproject/encoding/) { get; set; } | Gets and sets the encoding of VBA project. |
| [IslockedForViewing](../../aspose.cells.vba/vbaproject/islockedforviewing/) { get; } | Indicates whether this VBA project is locked for viewing. |
| [IsProtected](../../aspose.cells.vba/vbaproject/isprotected/) { get; } | Indicates whether this VBA project is protected. |
| [IsSigned](../../aspose.cells.vba/vbaproject/issigned/) { get; } | Indicates whether VBAcode is signed or not. |
| [IsValidSigned](../../aspose.cells.vba/vbaproject/isvalidsigned/) { get; } | Indicates whether the signature of VBA project is valid or not. |
| [Modules](../../aspose.cells.vba/vbaproject/modules/) { get; } | Gets all [`VbaModule`](../vbamodule/) objects. |
| [Name](../../aspose.cells.vba/vbaproject/name/) { get; set; } | Gets and sets the name of the VBA project. |
| [References](../../aspose.cells.vba/vbaproject/references/) { get; } | Gets all references of VBA project. |
## Methods
| Name | Description |
| --- | --- |
| [Copy](../../aspose.cells.vba/vbaproject/copy/)(VbaProject) | Copy VBA project from other file. |
| [Protect](../../aspose.cells.vba/vbaproject/protect/)(bool, string) | Protects or unprotects this VBA project. |
| [Sign](../../aspose.cells.vba/vbaproject/sign/)(DigitalSignature) | Sign this VBA project by a DigitalSignature |
| [ValidatePassword](../../aspose.cells.vba/vbaproject/validatepassword/)(string) | Validates protection password. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Vba;
using Aspose.Cells.DigitalSignatures;
using System;
using System.Text;
using System.Security.Cryptography.X509Certificates;
public class VbaProjectDemo
{
public static void VbaProjectExample()
{
// Instantiating a Workbook object
Workbook workbook = new Workbook();
// Init VBA project
VbaProject vbaProject = workbook.VbaProject;
// Setting properties
vbaProject.Name = "MyVbaProject";
vbaProject.Encoding = Encoding.UTF8;
// Checking read-only properties
bool isSigned = vbaProject.IsSigned;
bool isProtected = vbaProject.IsProtected;
bool isLockedForViewing = vbaProject.IslockedForViewing;
bool isValidSigned = vbaProject.IsValidSigned;
// Adding a VBA module
int moduleIndex = vbaProject.Modules.Add(VbaModuleType.Class, "MyModule");
// Adding a VBA project reference
vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
// Protecting the VBA project
vbaProject.Protect(true, "password");
// Signing the VBA project
X509Certificate2 certificate = new X509Certificate2("path_to_certificate.pfx", "certificate_password");
DigitalSignature digitalSignature = new DigitalSignature(certificate, "Signature Comments", DateTime.Now);
vbaProject.Sign(digitalSignature);
// Saving the Excel file
workbook.Save("VbaProjectExample.xlsm");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)
