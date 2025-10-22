##VbaProject.CertRawData
VbaProject property. Gets certificate raw data if this VBA project is signed
## VbaProject.CertRawData property
Gets certificate raw data if this VBA project is signed.
```csharp
public byte[] CertRawData { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Vba;
using System;
using System.IO;
public class VbaProjectPropertyCertRawDataDemo
{
public static void Run()
{
// Create a new workbook with VBA project
Workbook workbook = new Workbook();
// No need to create new VbaProject as Workbook already has one
// Access the VBA project
VbaProject vbaProject = workbook.VbaProject;
// Check if the VBA project is signed
if (vbaProject.IsSigned)
{
// Display certificate raw data if signed
byte[] certData = vbaProject.CertRawData;
Console.WriteLine("VBA Project is signed. Certificate raw data length: " + (certData != null ? certData.Length : 0));
// Example: Save certificate data to file if exists
if (certData != null && certData.Length > 0)
{
File.WriteAllBytes("VbaCertificate.cer", certData);
Console.WriteLine("Certificate saved to file.");
}
}
else
{
Console.WriteLine("VBA Project is not signed. CertRawData is not available.");
}
// Example scenario: Load a workbook with signed VBA project
string signedWorkbookPath = "SignedWithVba.xlsm";
if (File.Exists(signedWorkbookPath))
{
Workbook signedWorkbook = new Workbook(signedWorkbookPath);
VbaProject signedVbaProject = signedWorkbook.VbaProject;
if (signedVbaProject.IsSigned)
{
byte[] signedCertData = signedVbaProject.CertRawData;
Console.WriteLine("Loaded workbook's VBA certificate data length: " +
(signedCertData != null ? signedCertData.Length : 0));
}
}
// Save the workbook
workbook.Save("VbaProjectCertRawDataDemo.xlsx");
}
}
}
```
### See Also
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)
