---
title: MsoFillFormatHelper.Texture
second_title: Aspose.Cells for .NET API Reference
description: MsoFillFormatHelper property. Gets the texture fill type
type: docs
url: /net/aspose.cells.drawing/msofillformathelper/texture/
---
## MsoFillFormatHelper.Texture property

Gets the texture fill type.

```csharp
public TextureType Texture { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Reflection;

    public class MsoFillFormatHelperPropertyTextureDemo
    {
        public static void Run()
        {
            // Create a new workbook and get the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a label to make the example meaningful
            worksheet.Cells["A1"].Value = "Texture Property Demo";

            try
            {
                // Create an instance of MsoFillFormatHelper using reflection (no public constructor)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Display the current value of the Texture property (read-only)
                Console.WriteLine($"Current Texture type: {fillHelper.Texture}");

                // Demonstrate that the property is read-only by attempting to set it (commented out)
                // fillHelper.Texture = TextureType.Canvas; // This would cause a compilation error

                // Show all available texture types for reference
                Console.WriteLine("\nAvailable Texture Types:");
                foreach (TextureType textureType in Enum.GetValues(typeof(TextureType)))
                {
                    Console.WriteLine($"- {textureType}");
                }

                // Save the workbook to demonstrate successful execution
                workbook.Save("TextureDemo.xlsx");

                Console.WriteLine("\nTexture property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during Texture demo: {ex.Message}");
            }
        }
    }
}
```

### See Also

* enum [TextureType](../../texturetype/)
* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


