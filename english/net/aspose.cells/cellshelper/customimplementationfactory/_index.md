---
title: CellsHelper.CustomImplementationFactory
second_title: Aspose.Cells for .NET API Reference
description: CellsHelper property. Gets or sets the factory for creating instances with special implementation
type: docs
url: /net/aspose.cells/cellshelper/customimplementationfactory/
---
## CellsHelper.CustomImplementationFactory property

Gets or sets the factory for creating instances with special implementation.

```csharp
public static CustomImplementationFactory CustomImplementationFactory { get; set; }
```

### Examples

```csharp
// Called: var memoryStream = CellsHelper.CustomImplementationFactory.CreateMemoryStream();
public static void Property_CustomImplementationFactory()
        {
            // Setting properties of CellsHelper
            CellsHelper.SignificantDigits = 15;
            CellsHelper.DPI = 96.0;
            CellsHelper.StartupPath = &quot;C:\\Program Files\\Aspose\\Cells&quot;;
            CellsHelper.AltStartPath = &quot;D:\\Aspose\\Cells&quot;;
            CellsHelper.LibraryPath = &quot;E:\\Aspose\\Cells\\Library&quot;;
            CellsHelper.IsCloudPlatform = true;

            // Assuming CustomImplementationFactory is already defined and instantiated elsewhere
            CellsHelper.CustomImplementationFactory = new CustomImplementationFactory();

            // Demonstrating the use of CellsHelper properties
            Console.WriteLine(&quot;Significant Digits: &quot; + CellsHelper.SignificantDigits);
            Console.WriteLine(&quot;DPI: &quot; + CellsHelper.DPI);
            Console.WriteLine(&quot;Startup Path: &quot; + CellsHelper.StartupPath);
            Console.WriteLine(&quot;Alternate Startup Path: &quot; + CellsHelper.AltStartPath);
            Console.WriteLine(&quot;Library Path: &quot; + CellsHelper.LibraryPath);
            Console.WriteLine(&quot;Is Cloud Platform: &quot; + CellsHelper.IsCloudPlatform);

            // Example of using CustomImplementationFactory
            var memoryStream = CellsHelper.CustomImplementationFactory.CreateMemoryStream();
            Console.WriteLine(&quot;MemoryStream created with CustomImplementationFactory: &quot; + (memoryStream != null));

            return;
        }
```

### See Also

* class [CustomImplementationFactory](../../customimplementationfactory/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


