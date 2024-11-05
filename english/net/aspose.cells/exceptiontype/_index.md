---
title: Enum ExceptionType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.ExceptionType enum. Represents custom exception type code
type: docs
url: /net/aspose.cells/exceptiontype/
---
## ExceptionType enumeration

Represents custom exception type code.

```csharp
public enum ExceptionType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Chart | `0` | Invalid chart setting. |
| DataType | `1` | Invalid data type setting. |
| DataValidation | `2` | Invalid data validation setting. |
| ConditionalFormatting | `3` | Invalid data validation setting. |
| FileFormat | `4` | Invalid file format. |
| Formula | `5` | Invalid formula. |
| InvalidData | `6` | Invalid data. |
| InvalidOperator | `7` | Invalid operator. |
| IncorrectPassword | `8` | Incorrect password. |
| License | `9` | License related errors. |
| Limitation | `10` | Out of MS Excel limitation error. |
| PageSetup | `11` | Invalid page setup setting. |
| PivotTable | `12` | Invalid pivotTable setting. |
| Shape | `13` | Invalid drawing object setting. |
| Sparkline | `14` | Invalid sparkline object setting. |
| SheetName | `15` | Invalid worksheet name. |
| SheetType | `16` | Invalid worksheet type. |
| Interrupted | `17` | The process is interrupted. |
| IO | `18` | The file is invalid. |
| Permission | `19` | Permission is required to open this file. |
| UnsupportedFeature | `20` | Unsupported feature. |
| UnsupportedStream | `21` | Unsupported stream to be opened. |
| UndisclosedInformation | `22` | Files contains some undisclosed information. |
| FileCorrupted | `23` | File content is corrupted. |

### Examples

```csharp
[C#]

namespace Demos
{
    using Aspose.Cells;
    using System;

    public class ExceptionTypeDemo
    {
        public static void ExceptionTypeExample()
        {
            try
            {
                // Create a new workbook
                Workbook workbook = new Workbook();

                // Attempt to set an invalid worksheet name to trigger an exception
                workbook.Worksheets[0].Name = "Invalid/Name";

                // Save the workbook
                workbook.Save("ExceptionTypeExample.xlsx");
            }
            catch (CellsException ex)
            {
                // Handle the CellsException
                Console.WriteLine("An error occurred: " + ex.Message);
                Console.WriteLine("Exception Type Code: " + ex.Code);
                
                // Check the type of exception
                switch (ex.Code)
                {
                    case ExceptionType.SheetName:
                        Console.WriteLine("The worksheet name is invalid.");
                        break;
                    case ExceptionType.FileFormat:
                        Console.WriteLine("The file format is invalid.");
                        break;
                    // Add more cases as needed for different exception types
                    default:
                        Console.WriteLine("An unknown error occurred.");
                        break;
                }
            }
            catch (Exception ex)
            {
                // Handle any other exceptions
                Console.WriteLine("An unexpected error occurred: " + ex.Message);
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


