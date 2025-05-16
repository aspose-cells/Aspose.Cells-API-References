---
title: FontSettingCollection.Equals
second_title: Aspose.Cells for .NET API Reference
description: FontSettingCollection method. 
type: docs
url: /net/aspose.cells.drawing.texts/fontsettingcollection/equals/
---
## FontSettingCollection.Equals method

```csharp
public override bool Equals(object obj)
```

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object |  |

### Examples

```csharp
namespace AsposeCellsExamples.FontSettingCollectionMethodEqualsWithObjectDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add text to a cell and get its font settings
            worksheet.Cells["A1"].PutValue("Sample Text");
            FontSetting[] fontSettings1 = worksheet.Cells["A1"].GetCharacters();
            
            // Create another font setting array for comparison
            worksheet.Cells["A2"].PutValue("Sample Text");
            FontSetting[] fontSettings2 = worksheet.Cells["A2"].GetCharacters();
            
            // Create a different object for comparison
            object differentObject = new object();

            try
            {
                // Compare two identical font setting arrays
                bool result1 = fontSettings1.Equals(fontSettings2);
                Console.WriteLine($"Comparing identical collections: {result1}");
                
                // Compare with a different object
                bool result2 = fontSettings1.Equals(differentObject);
                Console.WriteLine($"Comparing with different object: {result2}");
                
                // Compare with null
                bool result3 = fontSettings1.Equals(null);
                Console.WriteLine($"Comparing with null: {result3}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }
            
            // Save the workbook
            workbook.Save("FontSettingCollectionEqualsDemo.xlsx");
        }
    }
}
```

### See Also

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


