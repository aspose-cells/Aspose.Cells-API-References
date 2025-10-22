##Aspose::Cells::Style class
'Aspose::Cells::Style class. Represents display style of excel document,such as font,color,alignment,border,etc. The Style object contains all style attributes (font, number format, alignment, and so on) as properties in C++.'
## Style class
Represents display style of excel document,such as font,color,alignment,border,etc. The [Style](./) object contains all style attributes (font, number format, alignment, and so on) as properties.
```cpp
class Style
```
## Methods
| Method | Description |
| --- | --- |
| [Copy(const Style\& style)](./copy/) | Copies data from another style object. |
| [Equals(const Aspose::Cells::Object\& obj)](./equals/) | Determines whether two [Style](./) instances are equal. |
| [GetBackgroundArgbColor()](./getbackgroundargbcolor/) | Gets and sets the background color with a 32-bit ARGB value. |
| [GetBackgroundColor()](./getbackgroundcolor/) | Gets or sets a style's background color. |
| [GetBackgroundThemeColor()](./getbackgroundthemecolor/) | Gets and sets the background theme color. |
| [GetBorders()](./getborders/) | Gets the [BorderCollection](../bordercollection/) of the style. |
| [GetCultureCustom()](./getculturecustom/) | Gets and sets the culture-dependent pattern string for number format. If no number format has been set for this object, null will be returned. If number format is builtin, the pattern string corresponding to the builtin number will be returned. |
| [GetCustom()](./getcustom/) | Represents the custom number format string of this style object. If the custom number format is not set(For example, the number format is builtin), "" will be returned. |
| [GetFont()](./getfont/) | Gets a [Font](../font/) object. |
| [GetForegroundArgbColor()](./getforegroundargbcolor/) | Gets and sets the foreground color with a 32-bit ARGB value. |
| [GetForegroundColor()](./getforegroundcolor/) | Gets or sets a style's foreground color. |
| [GetForegroundThemeColor()](./getforegroundthemecolor/) | Gets and sets the foreground theme color. |
| [GetHasBorders()](./gethasborders/) | Checks whether there are borders have been set for the style. |
| [GetHashCode()](./gethashcode/) | Serves as a hash function for a [Style](./) object. |
| [GetHorizontalAlignment()](./gethorizontalalignment/) | Gets or sets the horizontal alignment type of the text in a cell. |
| [GetIndentLevel()](./getindentlevel/) | Represents the indent level for the cell or range. Can only be an integer from 0 to 250. |
| [GetInvariantCustom()](./getinvariantcustom/) | Gets the culture-independent pattern string for number format. If no number format has been set for this object, null will be returned. If number format is builtin, the pattern string corresponding to the builtin number will be returned. |
| [GetName()](./getname/) | Gets or sets the name of the style. |
| [GetNumber()](./getnumber/) | Gets or sets the display format of numbers and dates. The formatting patterns are different for different regions. |
| [GetParentStyle()](./getparentstyle/) | Gets the parent style of this style. |
| [GetPattern()](./getpattern/) | Gets or sets the cell background pattern type. |
| [GetQuotePrefix()](./getquoteprefix/) | Indicates whether the cell's value starts with single quote mark. |
| [GetRotationAngle()](./getrotationangle/) | Represents text rotation angle. |
| [GetShrinkToFit()](./getshrinktofit/) | Represents if text automatically shrinks to fit in the available column width. |
| [GetTextDirection()](./gettextdirection/) | Represents text reading order. |
| [GetTwoColorGradientSetting()](./gettwocolorgradientsetting/) | Get the two-color gradient setting. |
| [GetVerticalAlignment()](./getverticalalignment/) | Gets or sets the vertical alignment type of the text in a cell. |
| [IsAlignmentApplied()](./isalignmentapplied/) | Indicate whether the alignment formatting should be applied. |
| [IsBorderApplied()](./isborderapplied/) | Indicate whether the border formatting should be applied. |
| [IsDateTime()](./isdatetime/) | Indicates whether the number format is a date format. |
| [IsFillApplied()](./isfillapplied/) | Indicate whether the fill formatting should be applied. |
| [IsFontApplied()](./isfontapplied/) | Indicate whether the font formatting should be applied. |
| [IsFormulaHidden()](./isformulahidden/) | Represents if the formula will be hidden when the worksheet is protected. |
| [IsGradient()](./isgradient/) | Indicates whether the cell shading is a gradient pattern. |
| [IsJustifyDistributed()](./isjustifydistributed/) | Indicates if the cells justified or distributed alignment should be used on the last line of text. |
| [IsLocked()](./islocked/) | Gets or sets a value indicating whether a cell can be modified or not. |
| [IsModified(StyleModifyFlag modifyFlag)](./ismodified/) | Checks whether the specified properties of the style have been modified. Used for style of ConditionalFormattings to check whether the specified properties of this style should be used when applying the ConditionalFormattings on a cell. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsNumberFormatApplied()](./isnumberformatapplied/) | Indicate whether the number formatting should be applied. |
| [IsPercent()](./ispercent/) | Indicates whether the number format is a percent format. |
| [IsProtectionApplied()](./isprotectionapplied/) | Indicate whether the protection formatting should be applied. |
| [IsTextWrapped()](./istextwrapped/) | Gets or sets a value indicating whether the text within a cell is wrapped. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const Style\& src)](./operator_asm/) | operator= |
| [SetBackgroundArgbColor(int32_t value)](./setbackgroundargbcolor/) | Gets and sets the background color with a 32-bit ARGB value. |
| [SetBackgroundColor(const Aspose::Cells::Color\& value)](./setbackgroundcolor/) | Gets or sets a style's background color. |
| [SetBackgroundThemeColor(const ThemeColor\& value)](./setbackgroundthemecolor/) | Gets and sets the background theme color. |
| [SetBorder(BorderType borderType, CellBorderType borderStyle, const Aspose::Cells::Color\& borderColor)](./setborder/) | Sets the borders of the style. |
| [SetBorder(BorderType borderType, CellBorderType borderStyle, const CellsColor\& borderColor)](./setborder/) | Sets the borders of the style. |
| [SetCultureCustom(const U16String\& value)](./setculturecustom/) | Gets and sets the culture-dependent pattern string for number format. If no number format has been set for this object, null will be returned. If number format is builtin, the pattern string corresponding to the builtin number will be returned. |
| [SetCultureCustom(const char16_t* value)](./setculturecustom/) | Gets and sets the culture-dependent pattern string for number format. If no number format has been set for this object, null will be returned. If number format is builtin, the pattern string corresponding to the builtin number will be returned. |
| [SetCustom(const U16String\& custom, bool builtinPreference)](./setcustom/) | Sets the Custom number format string of a cell. |
| [SetCustom(const char16_t* custom, bool builtinPreference)](./setcustom/) | Sets the Custom number format string of a cell. |
| [SetCustom(const U16String\& value)](./setcustom/) | Represents the custom number format string of this style object. If the custom number format is not set(For example, the number format is builtin), "" will be returned. |
| [SetCustom(const char16_t* value)](./setcustom/) | Represents the custom number format string of this style object. If the custom number format is not set(For example, the number format is builtin), "" will be returned. |
| [SetForegroundArgbColor(int32_t value)](./setforegroundargbcolor/) | Gets and sets the foreground color with a 32-bit ARGB value. |
| [SetForegroundColor(const Aspose::Cells::Color\& value)](./setforegroundcolor/) | Gets or sets a style's foreground color. |
| [SetForegroundThemeColor(const ThemeColor\& value)](./setforegroundthemecolor/) | Gets and sets the foreground theme color. |
| [SetHorizontalAlignment(TextAlignmentType value)](./sethorizontalalignment/) | Gets or sets the horizontal alignment type of the text in a cell. |
| [SetIndentLevel(int32_t value)](./setindentlevel/) | Represents the indent level for the cell or range. Can only be an integer from 0 to 250. |
| [SetIsAlignmentApplied(bool value)](./setisalignmentapplied/) | Indicate whether the alignment formatting should be applied. |
| [SetIsBorderApplied(bool value)](./setisborderapplied/) | Indicate whether the border formatting should be applied. |
| [SetIsFillApplied(bool value)](./setisfillapplied/) | Indicate whether the fill formatting should be applied. |
| [SetIsFontApplied(bool value)](./setisfontapplied/) | Indicate whether the font formatting should be applied. |
| [SetIsFormulaHidden(bool value)](./setisformulahidden/) | Represents if the formula will be hidden when the worksheet is protected. |
| [SetIsGradient(bool value)](./setisgradient/) | Indicates whether the cell shading is a gradient pattern. |
| [SetIsJustifyDistributed(bool value)](./setisjustifydistributed/) | Indicates if the cells justified or distributed alignment should be used on the last line of text. |
| [SetIsLocked(bool value)](./setislocked/) | Gets or sets a value indicating whether a cell can be modified or not. |
| [SetIsNumberFormatApplied(bool value)](./setisnumberformatapplied/) | Indicate whether the number formatting should be applied. |
| [SetIsProtectionApplied(bool value)](./setisprotectionapplied/) | Indicate whether the protection formatting should be applied. |
| [SetIsTextWrapped(bool value)](./setistextwrapped/) | Gets or sets a value indicating whether the text within a cell is wrapped. |
| [SetName(const U16String\& value)](./setname/) | Gets or sets the name of the style. |
| [SetName(const char16_t* value)](./setname/) | Gets or sets the name of the style. |
| [SetNumber(int32_t value)](./setnumber/) | Gets or sets the display format of numbers and dates. The formatting patterns are different for different regions. |
| [SetPattern(BackgroundType value)](./setpattern/) | Gets or sets the cell background pattern type. |
| [SetPatternColor(BackgroundType pattern, const Aspose::Cells::Color\& color1, const Aspose::Cells::Color\& color2)](./setpatterncolor/) | Sets the background color. |
| [SetQuotePrefix(bool value)](./setquoteprefix/) | Indicates whether the cell's value starts with single quote mark. |
| [SetRotationAngle(int32_t value)](./setrotationangle/) | Represents text rotation angle. |
| [SetShrinkToFit(bool value)](./setshrinktofit/) | Represents if text automatically shrinks to fit in the available column width. |
| [SetTextDirection(TextDirectionType value)](./settextdirection/) | Represents text reading order. |
| [SetTwoColorGradient(const Aspose::Cells::Color\& color1, const Aspose::Cells::Color\& color2, GradientStyleType gradientStyleType, int32_t variant)](./settwocolorgradient/) | Sets the specified fill to a two-color gradient. |
| [SetVerticalAlignment(TextAlignmentType value)](./setverticalalignment/) | Gets or sets the vertical alignment type of the text in a cell. |
| [Style(Style_Impl* impl)](./style/) | Constructs from an implementation object. |
| [Style(const Style\& src)](./style/) | Copy constructor. |
| [ToJson()](./tojson/) | Convert [Style](./) to JSON struct data. |
| [Update()](./update/) | Apply the named style to the styles of the cells which use this named style. It works like clicking the "ok" button after you finished modifying the style. Only applies for named style. |
| [~Style()](./~style/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
Workbook workbook;
WorksheetCollection sheets = workbook.GetWorksheets();
Cell cell = sheets.Get(0).GetCells().Get(u"A1");
Style style = cell.GetStyle();
style.GetFont().SetName(u"Times New Roman");
style.GetFont().SetColor(Color{ 0xff, 0, 0, 0xff });//Blue
cell.SetStyle(style);
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
