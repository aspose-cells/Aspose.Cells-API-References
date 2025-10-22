##FileFormatUtil.VerifyPassword
FileFormatUtil method. Detects and returns the information about a format of an excel stored in a stream
## FileFormatUtil.VerifyPassword method
Detects and returns the information about a format of an excel stored in a stream.
```csharp
public static bool VerifyPassword(Stream stream, string password)
```
| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream |  |
| password | String | The password for encrypted ooxml files. |
### Return Value
Returns whether the password is corrected.
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FileFormatUtilMethodVerifyPasswordWithStreamStringDemo
{
public static void Run()
{
string filePath = "example.xlsx";
string correctPassword = "test";
string wrongPassword = "1234";
using (Stream stream = File.OpenRead(filePath))
{
bool isValid = FileFormatUtil.VerifyPassword(stream, correctPassword);
Console.WriteLine($"Password '{correctPassword}' is valid: {isValid}");
}
using (Stream stream = File.OpenRead(filePath))
{
bool isValid = FileFormatUtil.VerifyPassword(stream, wrongPassword);
Console.WriteLine($"Password '{wrongPassword}' is valid: {isValid}");
}
}
}
}
```
### See Also
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
