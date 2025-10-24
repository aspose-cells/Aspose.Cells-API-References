##Cells.ImportCSV
Cells method. Import a CSV file to the cells
## ImportCSV(string, string, bool, int, int) {#importcsv_3}
Import a CSV file to the cells.
```csharp
public void ImportCSV(string fileName, string splitter, bool convertNumericData, int firstRow,
int firstColumn)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | The CSV file name. |
| splitter | String | The splitter |
| convertNumericData | Boolean | Whether the string in text file is converted to numeric data. |
| firstRow | Int32 | The row number of the first cell to import in. |
| firstColumn | Int32 | The column number of the first cell to import in. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodImportCSVWithStringStringBooleanInt32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Path to the CSV file
string csvPath = "example.csv";
// Import CSV data starting at cell A1 (row 0, column 0)
// Using semicolon as delimiter and converting numeric data
cells.ImportCSV(csvPath, ";", true, 0, 0);
// Save the workbook
workbook.Save("output.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## ImportCSV(Stream, string, bool, int, int) {#importcsv_1}
Import a CSV file to the cells.
```csharp
public void ImportCSV(Stream stream, string splitter, bool convertNumericData, int firstRow,
int firstColumn)
```
| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The CSV file stream. |
| splitter | String | The splitter |
| convertNumericData | Boolean | Whether the string in text file is converted to numeric data. |
| firstRow | Int32 | The row number of the first cell to import in. |
| firstColumn | Int32 | The column number of the first cell to import in. |
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## ImportCSV(string, TxtLoadOptions, int, int) {#importcsv_2}
Import a CSV file to the cells.
```csharp
public void ImportCSV(string fileName, TxtLoadOptions options, int firstRow, int firstColumn)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | The CSV file name. |
| options | TxtLoadOptions | The load options for reading text file |
| firstRow | Int32 | The row number of the first cell to import in. |
| firstColumn | Int32 | The column number of the first cell to import in. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodImportCSVWithStringTxtLoadOptionsInt32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create CSV load options
TxtLoadOptions loadOptions = new TxtLoadOptions();
loadOptions.Separator = ',';
loadOptions.ConvertDateTimeData = true;
loadOptions.ConvertNumericData = true;
loadOptions.ParsingFormulaOnOpen = true;
// Sample CSV file path (replace with actual path in your environment)
string csvFilePath = "example.csv";
// Import CSV data starting at cell A1 (row 0, column 0)
worksheet.Cells.ImportCSV(csvFilePath, loadOptions, 0, 0);
// Save the workbook
workbook.Save("output.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [TxtLoadOptions](../../txtloadoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## ImportCSV(Stream, TxtLoadOptions, int, int) {#importcsv}
Import a CSV file to the cells.
```csharp
public void ImportCSV(Stream stream, TxtLoadOptions options, int firstRow, int firstColumn)
```
| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The CSV file stream. |
| options | TxtLoadOptions | The load options for reading text file |
| firstRow | Int32 | The row number of the first cell to import in. |
| firstColumn | Int32 | The column number of the first cell to import in. |
### See Also
* class [TxtLoadOptions](../../txtloadoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
