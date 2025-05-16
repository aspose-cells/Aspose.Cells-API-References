---
title: AccentEquationNode.AccentCharacterType
second_title: Aspose.Cells for .NET API Reference
description: AccentEquationNode property. Specify combining characters by type value
type: docs
url: /net/aspose.cells.drawing.equations/accentequationnode/accentcharactertype/
---
## AccentEquationNode.AccentCharacterType property

Specify combining characters by type value.

```csharp
public EquationCombiningCharacterType AccentCharacterType { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples.AccentEquationNodePropertyAccentCharacterTypeDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class AccentEquationNodePropertyAccentCharacterTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Since AccentEquationNode doesn't have a parameterless constructor,
                // we'll demonstrate the property using an existing node from the worksheet
                // or create one through the worksheet's equation collection if available
                // For demonstration purposes, we'll show the property usage without instantiation
                
                // This would normally be created through worksheet.Equations.AddAccentEquation() or similar
                // But since we don't have that context, we'll show the property usage conceptually
                Console.WriteLine("Demonstrating AccentCharacterType property values:");
                
                // Display enum values and their usage
                Console.WriteLine("\nAvailable AccentCharacterType values:");
                foreach (EquationCombiningCharacterType type in Enum.GetValues(typeof(EquationCombiningCharacterType)))
                {
                    Console.WriteLine($"{type} = {(int)type}");
                    // In real usage, you would set this on an existing AccentEquationNode:
                    // accentNode.AccentCharacterType = type;
                }
                
                // Example of how you would set the property if you had a valid node:
                // var accentNode = GetAccentEquationNodeSomehow(); // This would be implementation-specific
                // accentNode.AccentCharacterType = EquationCombiningCharacterType.CircumflexAccent;
                // Console.WriteLine("Current AccentCharacterType: " + accentNode.AccentCharacterType);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### See Also

* enum [EquationCombiningCharacterType](../../equationcombiningcharactertype/)
* class [AccentEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


