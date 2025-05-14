---
title: FontConfigs.SetFontFolder
second_title: Aspose.Cells for .NET API Reference
description: FontConfigs method. Sets the fonts folder
type: docs
url: /net/aspose.cells/fontconfigs/setfontfolder/
---
## FontConfigs.SetFontFolder method

Sets the fonts folder

```csharp
public static void SetFontFolder(string fontFolder, bool recursive)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fontFolder | String | The folder that contains TrueType fonts. |
| recursive | Boolean | Determines whether or not to scan subfolders. |

### Examples

```csharp
// Called: FontConfigs.SetFontFolder("Fonts", true);
public void FontConfigs_Method_SetFontFolder()
{
    string path = Constants.TemplatePath + "NetCoreTests/CELLSNETCORE31/";

    Workbook wb = new Workbook(path + "example.xlsx");
    FontConfigs.SetFontFolder("Fonts", true);
    wb.Save(destPathNetCore + "example.pdf", SaveFormat.Pdf);//Error occurs here
}
```

### See Also

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


