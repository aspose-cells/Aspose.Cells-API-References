---
title: CellsHelper.SignificantDigits
second_title: Aspose.Cells for .NET API Reference
description: CellsHelper property. Gets and sets the number of significant digits. The default value is 17
type: docs
url: /net/aspose.cells/cellshelper/significantdigits/
---
## CellsHelper.SignificantDigits property

Gets and sets the number of significant digits. The default value is 17.

```csharp
public static int SignificantDigits { get; set; }
```

### Remarks

Only could be 15 or 17 now.

### Examples

```csharp
// Called: CellsHelper.SignificantDigits = 15;
public static void CellsHelper_Property_SignificantDigits()
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
```

### See Also

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


