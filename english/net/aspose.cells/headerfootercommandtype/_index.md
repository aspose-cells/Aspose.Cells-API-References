---
title: Enum HeaderFooterCommandType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.HeaderFooterCommandType enum. Represents the command type of header and footer
type: docs
url: /net/aspose.cells/headerfootercommandtype/
---
## HeaderFooterCommandType enumeration

Represents the command type of header and footer.

```csharp
public enum HeaderFooterCommandType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Text | `0` | The text. |
| CurrentPage | `1` | Current page number |
| Pagecount | `2` | Page count |
| CurrentDate | `3` | Current date |
| CurrentTime | `4` | Current time |
| SheetName | `5` | Sheet name |
| FileName | `6` | File name without path |
| FilePath | `7` | File path without file name |
| Picture | `8` | Picture |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassHeaderFooterCommandTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook for demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Set header with different command types
                worksheet.PageSetup.SetHeader(0, "&[Page] of &[Pages] - &[Date] - &[Time] - &[File]");

                // Retrieve header commands
                string headerScript = worksheet.PageSetup.GetHeader(0);
                HeaderFooterCommand[] commands = worksheet.PageSetup.GetCommands(headerScript);

                // Demonstrate different HeaderFooterCommandType values
                foreach (HeaderFooterCommand cmd in commands)
                {
                    Console.WriteLine($"Command Type: {cmd.Type}");

                    // Check for specific command types
                    if (cmd.Type == HeaderFooterCommandType.CurrentPage)
                    {
                        Console.WriteLine("Found CurrentPage command");
                    }
                    else if (cmd.Type == HeaderFooterCommandType.Pagecount)
                    {
                        Console.WriteLine("Found Pagecount command");
                    }
                    else if (cmd.Type == HeaderFooterCommandType.CurrentDate)
                    {
                        Console.WriteLine("Found CurrentDate command");
                    }
                    else if (cmd.Type == HeaderFooterCommandType.CurrentTime)
                    {
                        Console.WriteLine("Found CurrentTime command");
                    }
                    else if (cmd.Type == HeaderFooterCommandType.FileName)
                    {
                        Console.WriteLine("Found FileName command");
                    }
                }

                // Save the workbook to demonstrate header configuration
                workbook.Save("HeaderFooterCommandTypeDemo.xlsx");
                Console.WriteLine("HeaderFooterCommandType demonstration completed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with HeaderFooterCommandType: {ex.Message}");
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


