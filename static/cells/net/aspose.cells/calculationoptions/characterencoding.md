##CalculationOptions.CharacterEncoding
CalculationOptions property. Specifies the encoding used for encoding/decoding characters when calculating formulas. For functions such as CHAR CODE the calculated result depends on the region settings and default charset of the environment. With this property user can specify the proper encoding used for those function to get the expected result
## CalculationOptions.CharacterEncoding property
Specifies the encoding used for encoding/decoding characters when calculating formulas. For functions such as CHAR, CODE, the calculated result depends on the region settings and default charset of the environment. With this property user can specify the proper encoding used for those function to get the expected result.
```csharp
public Encoding CharacterEncoding { get; set; }
```
### Examples
```csharp
using System;
using System.Text;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CalculationOptionsPropertyCharacterEncodingDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
wb.Settings.Region = CountryCode.Japan;
CalculationOptions copts = new CalculationOptions();
copts.CharacterEncoding = Encoding.GetEncoding("iso-2022-jp");
string formula = "=TRIM(1)";
string result = (string)sheet.CalculateFormula(formula, copts);
Console.WriteLine("Calculation result: " + result);
}
}
}
```
### See Also
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
