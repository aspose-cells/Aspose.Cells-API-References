##Class License
Aspose.Cells.License class. Provides methods to license the component
## License class
Provides methods to license the component.
```csharp
public class License
```
## Constructors
| Name | Description |
| --- | --- |
| [License](license/)() | Initializes a new instance of this class. |
## Methods
| Name | Description |
| --- | --- |
| [SetLicense](../../aspose.cells/license/setlicense/#setlicense)(Stream) | Licenses the component. |
| [SetLicense](../../aspose.cells/license/setlicense/#setlicense_1)(string) | Licenses the component. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.IO;
public class LicenseDemo
{
public static void LicenseExample()
{
// Create an instance of the License class
License license = new License();
// Set the license using a license file name
license.SetLicense("Aspose.Cells.NET.lic");
// Alternatively, set the license using a stream
using (FileStream licenseStream = new FileStream("Aspose.Cells.NET.lic", FileMode.Open))
{
license.SetLicense(licenseStream);
}
// Additional code to demonstrate the usage of licensed Aspose.Cells functionality
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells[0, 0].PutValue("Hello, Aspose.Cells!");
// Save the workbook to verify the license is applied correctly
workbook.Save("LicensedWorkbook.xlsx");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
