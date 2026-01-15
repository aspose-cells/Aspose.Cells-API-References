---
title: IndividualFontConfigs.SetFontFolders
second_title: Aspose.Cells for .NET API Reference
description: IndividualFontConfigs method. Sets the font folders
type: docs
url: /net/aspose.cells/individualfontconfigs/setfontfolders/
---
## IndividualFontConfigs.SetFontFolders method

Sets the font folders

```csharp
public void SetFontFolders(string[] fontFolders, bool recursive)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fontFolders | String[] | The folders that contains TrueType fonts. |
| recursive | Boolean | Determines whether or not to scan subfolders. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IndividualFontConfigsMethodSetFontFoldersWithStringBooleanDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create an instance of IndividualFontConfigs
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // Prepare font folders array
            string[] fontFolders = new string[] { @"C:\Windows\Fonts", @"D:\CustomFonts" };
            bool recursiveSearch = true;

            try
            {
                // Call SetFontFolders method with String[] and Boolean parameters
                fontConfigs.SetFontFolders(fontFolders, recursiveSearch);

                // Demonstrate effect by using a custom font
                worksheet.Cells["A1"].PutValue("Text with custom font");
                Style style = worksheet.Cells["A1"].GetStyle();
                style.Font.Name = "SomeCustomFont"; // Assuming this font exists in one of the folders
                worksheet.Cells["A1"].SetStyle(style);

                Console.WriteLine("SetFontFolders method executed successfully with parameters (String[], Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFontFolders method: {ex.Message}");
            }

            // Save the result
            workbook.Save("SetFontFoldersDemo.xlsx");
        }
    }
}
```

### See Also

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


