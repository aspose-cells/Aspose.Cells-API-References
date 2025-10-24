##TxtLoadOptions.ExtendToNextSheet
TxtLoadOptions property. Whether extends data to next sheet when the rows or columns of data exceed limit. Default is false
## TxtLoadOptions.ExtendToNextSheet property
Whether extends data to next sheet when the rows or columns of data exceed limit. Default is false.
```csharp
public bool ExtendToNextSheet { get; set; }
```
### Remarks
If this property is true, extra data will be put into next sheet behind current one (if current sheet is the last one, new sheet will be appended to current workbook). If this property is false, the data exceeding limit will be ignored.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class TxtLoadOptionsPropertyExtendToNextSheetDemo
{
public static void Run()
{
// Create a sample CSV string that exceeds normal worksheet column limits
string csvData = "A,B,C,D,E,F,G,H,I,J,K,L,M,N,O,P,Q,R,S,T,U,V,W,X,Y,Z,AA,AB,AC,AD,AE,AF,AG,AH,AI,AJ,AK,AL,AM,AN,AO,AP,AQ,AR,AS,AT,AU,AV,AW,AX,AY,AZ,BA,BB,BC,BD,BE,BF,BG,BH,BI,BJ,BK,BL,BM,BN,BO,BP,BQ,BR,BS,BT,BU,BV,BW,BX,BY,BZ,CA,CB,CC,CD,CE,CF,CG,CH,CI,CJ,CK,CL,CM,CN,CO,CP,CQ,CR,CS,CT,CU,CV,CW,CX,CY,CZ,DA,DB,DC,DD,DE,DF,DG,DH,DI,DJ,DK,DL,DM,DN,DO,DP,DQ,DR,DS,DT,DU,DV,DW,DX,DY,DZ,EA,EB,EC,ED,EE,EF,EG,EH,EI,EJ,EK,EL,EM,EN,EO,EP,EQ,ER,ES,ET,EU,EV,EW,EX,EY,EZ";
// Create TxtLoadOptions with ExtendToNextSheet enabled
TxtLoadOptions options = new TxtLoadOptions
{
ExtendToNextSheet = true
};
// Create a workbook from the CSV data
Workbook workbook = new Workbook(new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData)), options);
// Get the cells from first worksheet
Cells cells = workbook.Worksheets[0].Cells;
// Output information about the imported data
Console.WriteLine("Number of worksheets: " + workbook.Worksheets.Count);
Console.WriteLine("Columns in first worksheet: " + workbook.Worksheets[0].Cells.MaxColumn);
if (workbook.Worksheets.Count > 1)
{
Console.WriteLine("Columns in second worksheet: " + workbook.Worksheets[1].Cells.MaxColumn);
Console.WriteLine("First cell in second worksheet: " + workbook.Worksheets[1].Cells[0, 0].StringValue);
}
}
}
}
```
### See Also
* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
