##CellsHelper.NeedQuoteInFormula
CellsHelper method. Indicates whether the name of the sheet should be enclosed in single quotes
## CellsHelper.NeedQuoteInFormula method
Indicates whether the name of the sheet should be enclosed in single quotes
```csharp
public static bool NeedQuoteInFormula(string sheetName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sheetName | String | The name of the sheet |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsHelperMethodNeedQuoteInFormulaWithStringDemo
{
public static void Run()
{
Console.WriteLine("NeedQuoteInFormula(\"Test Ab\"): " + CellsHelper.NeedQuoteInFormula("Test Ab"));
Console.WriteLine("NeedQuoteInFormula(\"A123\"): " + CellsHelper.NeedQuoteInFormula("A123"));
Console.WriteLine("NeedQuoteInFormula(\"Sheet1\"): " + CellsHelper.NeedQuoteInFormula("Sheet1"));
}
}
}
```
### See Also
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
