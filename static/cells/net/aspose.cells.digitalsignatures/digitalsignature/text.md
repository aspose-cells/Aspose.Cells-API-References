##DigitalSignature.Text
DigitalSignature property. Specifies the text of actual signature in the digital signature. Default value is Empty
## DigitalSignature.Text property
Specifies the text of actual signature in the digital signature. Default value is Empty.
```csharp
public string Text { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;
using System;
using System.Security.Cryptography.X509Certificates;
public class DigitalSignaturePropertyTextDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a test certificate (in real scenario, use a valid certificate)
X509Certificate2 certificate = null;
try
{
certificate = new X509Certificate2();
}
catch
{
Console.WriteLine("Could not create certificate. Using null for demonstration.");
}
// Create a digital signature instance
DigitalSignature signature = new DigitalSignature(
certificate,
"Sample signature comments",
DateTime.Now);
// Display the current Text value (default is empty)
Console.WriteLine("Current Text value: " + signature.Text);
// Set a new value for the Text property
signature.Text = "Approved by John Doe";
// Create a digital signature collection and add the signature to it
DigitalSignatureCollection signatures = new DigitalSignatureCollection();
signatures.Add(signature);
// Add the digital signatures to the workbook
workbook.AddDigitalSignature(signatures);
// Save the workbook with digital signature
try
{
workbook.Save("DigitalSignatureWithText.xlsx");
Console.WriteLine("Workbook saved with digital signature text: " + signature.Text);
}
catch (Exception ex)
{
Console.WriteLine("Error saving workbook: " + ex.Message);
}
}
}
}
```
### See Also
* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)
