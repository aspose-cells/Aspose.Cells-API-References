---
title: CellsException.Code
second_title: Aspose.Cells for .NET API Reference
description: CellsException property. Represents custom exception code
type: docs
url: /net/aspose.cells/cellsexception/code/
---
## CellsException.Code property

Represents custom exception code.

```csharp
public ExceptionType Code { get; }
```

### Examples

```csharp
// Called: switch (ex.Code)
public static void Property_Code()
        {
            try
            {
                // Create a new workbook
                Workbook workbook = new Workbook();

                // Attempt to set an invalid worksheet name to trigger an exception
                workbook.Worksheets[0].Name = &quot;Invalid/Name&quot;;

                // Save the workbook
                workbook.Save(&quot;ExceptionTypeExample.xlsx&quot;);
            }
            catch (CellsException ex)
            {
                // Handle the CellsException
                Console.WriteLine(&quot;An error occurred: &quot; + ex.Message);
                Console.WriteLine(&quot;Exception Type Code: &quot; + ex.Code);
                
                // Check the type of exception
                switch (ex.Code)
                {
                    case ExceptionType.SheetName:
                        Console.WriteLine(&quot;The worksheet name is invalid.&quot;);
                        break;
                    case ExceptionType.FileFormat:
                        Console.WriteLine(&quot;The file format is invalid.&quot;);
                        break;
                    // Add more cases as needed for different exception types
                    default:
                        Console.WriteLine(&quot;An unknown error occurred.&quot;);
                        break;
                }
            }
            catch (Exception ex)
            {
                // Handle any other exceptions
                Console.WriteLine(&quot;An unexpected error occurred: &quot; + ex.Message);
            }
        }
```

### See Also

* enum [ExceptionType](../../exceptiontype/)
* class [CellsException](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


