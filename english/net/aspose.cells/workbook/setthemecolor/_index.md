---
title: Workbook.SetThemeColor
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Sets the theme color
type: docs
url: /net/aspose.cells/workbook/setthemecolor/
---
## Workbook.SetThemeColor method

Sets the theme color

```csharp
public void SetThemeColor(ThemeColorType type, Color color)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | ThemeColorType | The theme color type. |
| color | Color | the theme color |

### Examples

```csharp
// Called: workbook.SetThemeColor(ThemeColorType.Text1, Color.Green);
public void Workbook_Method_SetThemeColor()
{
    Console.WriteLine("Workbook_Method_SetThemeColor()");
    string infn = path + "Test_ExpThemeData.xlsx";
    string outfn = Constants.destPath + "Test_ExpThemeData_out.xlsx";

    Workbook workbook = new Workbook(infn);
    workbook.SetThemeColor(ThemeColorType.Background1, Color.Red);
    workbook.Save(outfn);

    infn = path + "Test_ExpThemeData_WithRel.xlsx";
    outfn = Constants.destPath + "Test_ExpThemeData_WithRel_out.xlsx";

    workbook = new Workbook(infn);
    workbook.SetThemeColor(ThemeColorType.Text1, Color.Yellow);
    workbook.Save(outfn);

    outfn = Constants.destPath + "Test_ExpThemeData_AddTheme.xlsx";

    workbook = new Workbook();

    workbook.SetThemeColor(ThemeColorType.Text1, Color.Green);
    Style s = workbook.DefaultStyle;
    s.Font.ThemeColor = new ThemeColor(ThemeColorType.Text1, 0);
    workbook.DefaultStyle = s;
    workbook.Save(outfn);

}
```

### See Also

* enum [ThemeColorType](../../themecolortype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


