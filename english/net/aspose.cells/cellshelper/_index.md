---
title: Class CellsHelper
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.CellsHelper class. Provides helper functions
type: docs
url: /net/aspose.cells/cellshelper/
---
## CellsHelper class

Provides helper functions.

```csharp
public class CellsHelper
```

## Properties

| Name | Description |
| --- | --- |
| static [AltStartPath](../../aspose.cells/cellshelper/altstartpath/) { get; set; } | Gets or sets the alternate startup path, which is referred to by some external formula references. |
| static [CustomImplementationFactory](../../aspose.cells/cellshelper/customimplementationfactory/) { get; set; } | Gets or sets the factory for creating instances with special implementation. |
| static [DPI](../../aspose.cells/cellshelper/dpi/) { get; set; } | Gets the DPI of the machine. |
| static [IsCloudPlatform](../../aspose.cells/cellshelper/iscloudplatform/) { get; set; } | Please set this property True when running on a cloud platform, such as: Azure, AWSLambda, etc, |
| static [LibraryPath](../../aspose.cells/cellshelper/librarypath/) { get; set; } | Gets or sets the library path which is referred to by some external formula references. |
| static [SignificantDigits](../../aspose.cells/cellshelper/significantdigits/) { get; set; } | (**Obsolete.**) Gets and sets the number of significant digits. The default value is 17. |
| static [SignificantDigitsType](../../aspose.cells/cellshelper/significantdigitstype/) { get; set; } | Gets and sets the default type of significant digits for outputing numeric values. Default value is G17. |
| static [StartupPath](../../aspose.cells/cellshelper/startuppath/) { get; set; } | Gets or sets the startup path, which is referred to by some external formula references. |

## Methods

| Name | Description |
| --- | --- |
| static [AddAddInFunction](../../aspose.cells/cellshelper/addaddinfunction/)(string, int, int, ParameterType[], ParameterType) | (**Obsolete.**) Add addin function. |
| static [CellIndexToName](../../aspose.cells/cellshelper/cellindextoname/)(int, int) | Gets cell name according to its row and column indexes. |
| static [CellNameToIndex](../../aspose.cells/cellshelper/cellnametoindex/)(string, out int, out int) | Gets the cell row and column indexes according to its name. |
| static [ColumnIndexToName](../../aspose.cells/cellshelper/columnindextoname/)(int) | Gets column name according to column index. |
| static [ColumnNameToIndex](../../aspose.cells/cellshelper/columnnametoindex/)(string) | Gets column index according to column name. |
| static [ConvertA1FormulaToR1C1](../../aspose.cells/cellshelper/converta1formulator1c1/)(string, int, int) | (**Obsolete.**) Converts A1 formula of the cell to the r1c1 formula. |
| static [ConvertR1C1FormulaToA1](../../aspose.cells/cellshelper/convertr1c1formulatoa1/)(string, int, int) | (**Obsolete.**) Converts the r1c1 formula of the cell to A1 formula. |
| static [CreateSafeSheetName](../../aspose.cells/cellshelper/createsafesheetname/#createsafesheetname)(string) | Checks given sheet name and create a valid one when needed. If given sheet name conforms to the rules of excel sheet name, then return it. Otherwise string will be truncated if length exceeds the limit and invalid characters will be replaced with ' ', then return the rebuilt string value. |
| static [CreateSafeSheetName](../../aspose.cells/cellshelper/createsafesheetname/#createsafesheetname_1)(string, char) | Checks given sheet name and create a valid one when needed. If given sheet name conforms to the rules of excel sheet name, then return it. Otherwise string will be truncated if length exceeds the limit and invalid characters will be replaced with given character, then return the rebuilt string value. |
| static [GetCacheFolder](../../aspose.cells/cellshelper/getcachefolder/)() | Gets the folder for temporary files that may be used as data cache. |
| static [GetDateTimeFromDouble](../../aspose.cells/cellshelper/getdatetimefromdouble/)(double, bool) | Convert the double value to the date time value. |
| static [GetDoubleFromDateTime](../../aspose.cells/cellshelper/getdoublefromdatetime/)(DateTime, bool) | Convert the date time to double value. |
| static [GetTextWidth](../../aspose.cells/cellshelper/gettextwidth/)(string, Font, double) | Get width of text in unit of points. |
| static [GetUsedColors](../../aspose.cells/cellshelper/getusedcolors/)(Workbook) | Gets all used colors in the workbook. |
| static [GetVersion](../../aspose.cells/cellshelper/getversion/)() | Get the release version. |
| static [MergeFiles](../../aspose.cells/cellshelper/mergefiles/)(string[], string, string) | Merges some large xls files to a xls file. |
| static [NeedQuoteInFormula](../../aspose.cells/cellshelper/needquoteinformula/)(string) | Indicates whether the name of the sheet should be enclosed in single quotes |
| static [RowIndexToName](../../aspose.cells/cellshelper/rowindextoname/)(int) | Gets row name according to row index. |
| static [RowNameToIndex](../../aspose.cells/cellshelper/rownametoindex/)(string) | Gets row index according to row name. |
| static [SetCacheFolder](../../aspose.cells/cellshelper/setcachefolder/)(string) | Sets the folder for temporary files that may be used as data cache. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperDemo
    {
        public static void CellsHelperExample()
        {
            // Setting properties of CellsHelper
            CellsHelper.SignificantDigits = 15;
            CellsHelper.DPI = 96.0;
            CellsHelper.StartupPath = "C:\\Program Files\\Aspose\\Cells";
            CellsHelper.AltStartPath = "D:\\Aspose\\Cells";
            CellsHelper.LibraryPath = "E:\\Aspose\\Cells\\Library";
            CellsHelper.IsCloudPlatform = true;

            // Assuming CustomImplementationFactory is already defined and instantiated elsewhere
            CellsHelper.CustomImplementationFactory = new CustomImplementationFactory();

            // Demonstrating the use of CellsHelper properties
            Console.WriteLine("Significant Digits: " + CellsHelper.SignificantDigits);
            Console.WriteLine("DPI: " + CellsHelper.DPI);
            Console.WriteLine("Startup Path: " + CellsHelper.StartupPath);
            Console.WriteLine("Alternate Startup Path: " + CellsHelper.AltStartPath);
            Console.WriteLine("Library Path: " + CellsHelper.LibraryPath);
            Console.WriteLine("Is Cloud Platform: " + CellsHelper.IsCloudPlatform);

            // Example of using CustomImplementationFactory
            var memoryStream = CellsHelper.CustomImplementationFactory.CreateMemoryStream();
            Console.WriteLine("MemoryStream created with CustomImplementationFactory: " + (memoryStream != null));

            return;
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


