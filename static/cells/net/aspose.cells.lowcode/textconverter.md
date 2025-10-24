##Class TextConverter
Aspose.Cells.LowCode.TextConverter class. Converter for conversion between text based formatscsv tsv dif... and other spreadsheet file formats
## TextConverter class
Converter for conversion between text based formats(csv, tsv, dif...) and other spreadsheet file formats.
```csharp
public class TextConverter
```
## Methods
| Name | Description |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/textconverter/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions) | Converts file format between text based formats and other spreadsheet file formats |
| static [Process](../../aspose.cells.lowcode/textconverter/process/#process_1)(string, string) | Converts given template file between text based files and other formats. |
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;
namespace AsposeCellsExamples
{
public class TextConverterDemo
{
public static void Process(string inputFile, string outputFile)
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
string[] lines = File.ReadAllLines(inputFile);
for (int i = 0; i < lines.Length; i++)
{
string[] cells = lines[i].Split(',');
for (int j = 0; j < cells.Length; j++)
{
worksheet.Cells[i, j].PutValue(cells[j]);
}
}
workbook.Save(outputFile, SaveFormat.Xlsx);
}
}
public class LowCodeClassTextConverterDemo
{
public static void Run()
{
TextConverter.Process("template.csv", "res.xlsx");
Console.WriteLine("Conversion completed successfully.");
}
}
}
```
### See Also
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)
