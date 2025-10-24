##MetadataOptions.MetadataType
MetadataOptions property. Gets and sets the type of the metadata which is loading
## MetadataOptions.MetadataType property
Gets and sets the type of the metadata which is loading.
```csharp
public MetadataType MetadataType { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Metadata;
using System;
public class MetadataOptionsPropertyMetadataTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Confidential Data");
MetadataOptions encryptOptions = new MetadataOptions(MetadataType.Encryption);
Console.WriteLine("Encryption MetadataType: " + encryptOptions.MetadataType);
encryptOptions.Password = "secret";
encryptOptions.KeyLength = 128;
XlsSaveOptions saveOptions = new XlsSaveOptions();
// Encryption options applied through workbook settings
workbook.SetEncryptionOptions(EncryptionType.StrongCryptographicProvider, encryptOptions.KeyLength);
workbook.Settings.Password = encryptOptions.Password;
workbook.Save("PropertyMetadataTypeDemo.xls", saveOptions);
MetadataOptions decryptOptions = new MetadataOptions(MetadataType.Decryption);
Console.WriteLine("Decryption MetadataType: " + decryptOptions.MetadataType);
decryptOptions.Password = "secret";
LoadOptions loadOptions = new LoadOptions(LoadFormat.Excel97To2003);
loadOptions.Password = decryptOptions.Password;
Workbook decryptedWorkbook = new Workbook("PropertyMetadataTypeDemo.xls", loadOptions);
Console.WriteLine("Decrypted value: " + decryptedWorkbook.Worksheets[0].Cells["A1"].StringValue);
}
}
}
```
### See Also
* enum [MetadataType](../../metadatatype/)
* class [MetadataOptions](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)
