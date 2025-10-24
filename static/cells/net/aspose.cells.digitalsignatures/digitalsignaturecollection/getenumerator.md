##DigitalSignatureCollection.GetEnumerator
DigitalSignatureCollection method. Get the enumerator for DigitalSignatureCollection this enumerator allows iteration over the collection
## DigitalSignatureCollection.GetEnumerator method
Get the enumerator for DigitalSignatureCollection, this enumerator allows iteration over the collection
```csharp
public IEnumerator GetEnumerator()
```
### Return Value
The enumerator to iteration.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;
using System;
using System.Collections;
using System.Security.Cryptography.X509Certificates;
public class DigitalSignatureCollectionMethodGetEnumeratorDemo
{
public static void Run()
{
// Create a new digital signature collection
DigitalSignatureCollection signatures = new DigitalSignatureCollection();
// Create sample digital signatures with required parameters
DigitalSignature signature1 = new DigitalSignature(
new X509Certificate2(), "Sample comment 1", DateTime.Now);
DigitalSignature signature2 = new DigitalSignature(
new X509Certificate2(), "Sample comment 2", DateTime.Now);
// Add signatures to the collection
signatures.Add(signature1);
signatures.Add(signature2);
try
{
// Get the enumerator
IEnumerator enumerator = signatures.GetEnumerator();
Console.WriteLine("Iterating through digital signatures:");
int count = 0;
while (enumerator.MoveNext())
{
DigitalSignature current = (DigitalSignature)enumerator.Current;
Console.WriteLine($"Signature #{++count} found");
}
Console.WriteLine($"Total signatures: {count}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetEnumerator method: {ex.Message}");
}
}
}
}
```
### See Also
* class [DigitalSignatureCollection](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)
