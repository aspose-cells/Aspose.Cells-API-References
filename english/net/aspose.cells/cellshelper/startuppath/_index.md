---
title: CellsHelper.StartupPath
second_title: Aspose.Cells for .NET API Reference
description: CellsHelper property. Gets or sets the startup path which is referred to by some external formula references
type: docs
url: /net/aspose.cells/cellshelper/startuppath/
---
## CellsHelper.StartupPath property

Gets or sets the startup path, which is referred to by some external formula references.

```csharp
public static string StartupPath { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine(&amp;quot;Startup Path: &amp;quot; + CellsHelper.StartupPath);
public static void Property_StartupPath()
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

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


