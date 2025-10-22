##Enum EncryptionType
Aspose.Cells.EncryptionType enum. Encryption Type. Only used by excel2003. We will encrypt 2007/2010 workbook using SHA AES the same as Excel does and this EncryptionType will be ignored
## EncryptionType enumeration
Encryption Type. Only used by excel2003. We will encrypt 2007/2010 workbook using SHA AES the same as Excel does, and this EncryptionType will be ignored.
```csharp
public enum EncryptionType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| XOR | `0` | XOR encryption algorithm. |
| Compatible | `1` | Office 97/2000 compatible. |
| EnhancedCryptographicProviderV1 | `2` | Enhanced encryption. |
| StrongCryptographicProvider | `3` | Strong encryption algorithm. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class EncryptionTypeDemo
{
public static void EncryptionTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Set encryption options for the workbook
EncryptionType encryptionType = EncryptionType.EnhancedCryptographicProviderV1;
int keyLength = 128; // Key length can be 40, 128, or 256 bits
// Apply encryption settings
workbook.SetEncryptionOptions(encryptionType, keyLength);
// Protect the workbook with a password
string password = "securePassword";
workbook.Protect(ProtectionType.All, password);
// Save the workbook
workbook.Save("EncryptedWorkbook.xlsx");
workbook.Save("EncryptedWorkbook.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
