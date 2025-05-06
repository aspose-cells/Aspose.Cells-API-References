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
// Called: FontConfigs.SetFontFolder(&amp;quot;Fonts&amp;quot;, true);
[Test]
        public void Method_Boolean_()
        {
            string path = Constants.TemplatePath + &quot;NetCoreTests/CELLSNETCORE31/&quot;;

            Workbook wb = new Workbook(path + &quot;CELLSNETCORE31.xlsx&quot;);
            FontConfigs.SetFontFolder(&quot;Fonts&quot;, true);
            wb.Save(destPathNetCore + &quot;CELLSNETCORE31_out.pdf&quot;, SaveFormat.Pdf);//Error occurs here
        }
```

### See Also

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


