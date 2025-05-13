---
title: Class FontConfigs
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.FontConfigs class. Specifies font settings
type: docs
url: /net/aspose.cells/fontconfigs/
---
## FontConfigs class

Specifies font settings

```csharp
public class FontConfigs
```

## Constructors

| Name | Description |
| --- | --- |
| [FontConfigs](fontconfigs/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| static [DefaultFontName](../../aspose.cells/fontconfigs/defaultfontname/) { get; set; } | Gets or sets the default font name. |
| static [PreferSystemFontSubstitutes](../../aspose.cells/fontconfigs/prefersystemfontsubstitutes/) { get; set; } | Indicate whether to use system font substitutes first or not when a font is not presented and the substitute of this font is not set. e.g. On Ubuntu, "Arial" font is generally substituted by "Liberation Sans". Default value is false. |

## Methods

| Name | Description |
| --- | --- |
| static [GetFontFileDataInfo](../../aspose.cells/fontconfigs/getfontfiledatainfo/)(string, bool, bool, bool) | Get data infomation of font file data. |
| static [GetFontSources](../../aspose.cells/fontconfigs/getfontsources/)() | Gets a copy of the array that contains the list of sources |
| static [GetFontSubstitutes](../../aspose.cells/fontconfigs/getfontsubstitutes/)(string) | Returns array containing font substitute names to be used if original font is not presented. |
| static [IsFontAvailable](../../aspose.cells/fontconfigs/isfontavailable/)(string) | Indicate whether the font is available. |
| static [SetFontFolder](../../aspose.cells/fontconfigs/setfontfolder/)(string, bool) | Sets the fonts folder |
| static [SetFontFolders](../../aspose.cells/fontconfigs/setfontfolders/)(string[], bool) | Sets the fonts folders |
| static [SetFontSources](../../aspose.cells/fontconfigs/setfontsources/)(FontSourceBase[]) | Sets the fonts sources. |
| static [SetFontSubstitutes](../../aspose.cells/fontconfigs/setfontsubstitutes/)(string, string[]) | Font substitute names for given original font name. |

### Examples

```csharp
// Called: FontConfigs.SetFontFolder(fontFolder, true);
public void Cells_Type_FontConfigs()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"JAVA42899/";

    String fontFolder = filePath + "font";
    FontConfigs.SetFontFolder(fontFolder, true);

    //Load the sample Excel file
    Workbook workbook = new Workbook(filePath + "test.xlsx");
    //Specify Html Save Options
    HtmlSaveOptions options = new HtmlSaveOptions();
    //We do not want to export document, workbook and worksheet properties
    options.ExportDocumentProperties = false;
    options.ExportWorkbookProperties = false;
    options.ExportWorksheetProperties = false;
    options.ExportSimilarBorderStyle = true;
    options.ExportImagesAsBase64 = false;
    options.ExcludeUnusedStyles = true;
    options.ExportHiddenWorksheet = false;
    options.WidthScalable = false;
    options.PresentationPreference = true;
    //Specify HtmlSaveOptions - Hide Overlaid Content with CrossHideRight while saving to Html
    options.HtmlCrossStringType = HtmlCrossType.CrossHideRight;
    //Export the Excel file to Html with Html Save Options

    workbook.Save(CreateFolder(filePath) + "out.html", options);
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


