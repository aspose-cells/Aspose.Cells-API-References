##Style Class
'Style class. Encapsulates the object that represents style in Go.'
## Style class
Represents display style of excel document,such as font,color,alignment,border,etc.The Style object contains all style attributes (font, number format, alignment, and so on) as properties.
```go
type Style struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetBackgroundThemeColor](./getbackgroundthemecolor/) | Gets and sets the background theme color. |
|[SetBackgroundThemeColor](./setbackgroundthemecolor/) | Gets and sets the background theme color. |
|[GetForegroundThemeColor](./getforegroundthemecolor/) | Gets and sets the foreground theme color. |
|[SetForegroundThemeColor](./setforegroundthemecolor/) | Gets and sets the foreground theme color. |
|[GetName](./getname/) | Gets or sets the name of the style. |
|[SetName](./setname/) | Gets or sets the name of the style. |
|[GetPattern](./getpattern/) | Gets or sets the cell background pattern type. |
|[SetPattern](./setpattern/) | Gets or sets the cell background pattern type. |
|[SetPatternColor](./setpatterncolor/) | Sets the background color. |
|[GetBorders](./getborders/) | Gets the BorderCollection of the style. |
|[GetBackgroundColor](./getbackgroundcolor/) | Gets or sets a style's background color. |
|[SetBackgroundColor](./setbackgroundcolor/) | Gets or sets a style's background color. |
|[GetBackgroundArgbColor](./getbackgroundargbcolor/) | Gets and sets the background color with a 32-bit ARGB value. |
|[SetBackgroundArgbColor](./setbackgroundargbcolor/) | Gets and sets the background color with a 32-bit ARGB value. |
|[GetForegroundColor](./getforegroundcolor/) | Gets or sets a style's foreground color. |
|[SetForegroundColor](./setforegroundcolor/) | Gets or sets a style's foreground color. |
|[GetForegroundArgbColor](./getforegroundargbcolor/) | Gets and sets the foreground color with a 32-bit ARGB value. |
|[SetForegroundArgbColor](./setforegroundargbcolor/) | Gets and sets the foreground color with a 32-bit ARGB value. |
|[Copy](./copy/) | Copies data from another style object |
|[GetHasBorders](./gethasborders/) | Checks whether there are borders have been set for the style. |
|[GetParentStyle](./getparentstyle/) | Gets the parent style of this style. |
|[Update](./update/) | Apply the named style to the styles of the cells which use this named style.It works like clicking the "ok" button after you finished modifying the style.Only applies for named style. |
|[IsNumberFormatApplied](./isnumberformatapplied/) | Indicate whether the number formatting should be applied. |
|[SetIsNumberFormatApplied](./setisnumberformatapplied/) | Indicate whether the number formatting should be applied. |
|[IsFontApplied](./isfontapplied/) | Indicate whether the font formatting should be applied. |
|[SetIsFontApplied](./setisfontapplied/) | Indicate whether the font formatting should be applied. |
|[IsAlignmentApplied](./isalignmentapplied/) | Indicate whether the alignment formatting should be applied. |
|[SetIsAlignmentApplied](./setisalignmentapplied/) | Indicate whether the alignment formatting should be applied. |
|[IsBorderApplied](./isborderapplied/) | Indicate whether the border formatting should be applied. |
|[SetIsBorderApplied](./setisborderapplied/) | Indicate whether the border formatting should be applied. |
|[IsFillApplied](./isfillapplied/) | Indicate whether the fill formatting should be applied. |
|[SetIsFillApplied](./setisfillapplied/) | Indicate whether the fill formatting should be applied. |
|[IsProtectionApplied](./isprotectionapplied/) | Indicate whether the protection formatting should be applied. |
|[SetIsProtectionApplied](./setisprotectionapplied/) | Indicate whether the protection formatting should be applied. |
|[IsModified](./ismodified/) | Checks whether the specified properties of the style have been modified.Used for style of ConditionalFormattings to check whether the specified properties of this style should be used when applying the ConditionalFormattings on a cell. |
|[Equals](./equals/) | Determines whether two Style instances are equal. |
|[GetHashCode](./gethashcode/) | Serves as a hash function for a Style object. |
|[GetIndentLevel](./getindentlevel/) | Represents the indent level for the cell or range. Can only be an integer from 0 to 250. |
|[SetIndentLevel](./setindentlevel/) | Represents the indent level for the cell or range. Can only be an integer from 0 to 250. |
|[GetFont](./getfont/) | Gets a Font object. |
|[GetRotationAngle](./getrotationangle/) | Represents text rotation angle. |
|[SetRotationAngle](./setrotationangle/) | Represents text rotation angle. |
|[GetHorizontalAlignment](./gethorizontalalignment/) | Gets or sets the horizontal alignment type of the text in a cell. |
|[SetHorizontalAlignment](./sethorizontalalignment/) | Gets or sets the horizontal alignment type of the text in a cell. |
|[GetVerticalAlignment](./getverticalalignment/) | Gets or sets the vertical alignment type of the text in a cell. |
|[SetVerticalAlignment](./setverticalalignment/) | Gets or sets the vertical alignment type of the text in a cell. |
|[IsTextWrapped](./istextwrapped/) | Gets or sets a value indicating whether the text within a cell is wrapped. |
|[SetIsTextWrapped](./setistextwrapped/) | Gets or sets a value indicating whether the text within a cell is wrapped. |
|[GetNumber](./getnumber/) | Gets or sets the display format of numbers and dates. The formatting patterns are different for different regions. |
|[SetNumber](./setnumber/) | Gets or sets the display format of numbers and dates. The formatting patterns are different for different regions. |
|[SetBorder_BorderType_CellBorderType_Color](./setborder_bordertype_cellbordertype_color/) | Sets the borders of the style. |
|[SetBorder_BorderType_CellBorderType_CellsColor](./setborder_bordertype_cellbordertype_cellscolor/) | Sets the borders of the style. |
|[IsLocked](./islocked/) | Gets or sets a value indicating whether a cell can be modified or not. |
|[SetIsLocked](./setislocked/) | Gets or sets a value indicating whether a cell can be modified or not. |
|[SetCustom_String_Bool](./setcustom_string_bool/) | Sets the Custom number format string of a cell. |
|[GetCustom](./getcustom/) | Represents the custom number format string of this style object.If the custom number format is not set(For example, the number format is builtin), "" will be returned. |
|[SetCustom_String](./setcustom_string/) | Represents the custom number format string of this style object.If the custom number format is not set(For example, the number format is builtin), "" will be returned. |
|[GetCultureCustom](./getculturecustom/) | Gets and sets the culture-dependent pattern string for number format.If no number format has been set for this object, null will be returned.If number format is builtin, the pattern string corresponding to the builtin number will be returned. |
|[SetCultureCustom](./setculturecustom/) | Gets and sets the culture-dependent pattern string for number format.If no number format has been set for this object, null will be returned.If number format is builtin, the pattern string corresponding to the builtin number will be returned. |
|[GetInvariantCustom](./getinvariantcustom/) | Gets the culture-independent pattern string for number format.If no number format has been set for this object, null will be returned.If number format is builtin, the pattern string corresponding to the builtin number will be returned. |
|[IsFormulaHidden](./isformulahidden/) | Represents if the formula will be hidden when the worksheet is protected. |
|[SetIsFormulaHidden](./setisformulahidden/) | Represents if the formula will be hidden when the worksheet is protected. |
|[GetShrinkToFit](./getshrinktofit/) | Represents if text automatically shrinks to fit in the available column width. |
|[SetShrinkToFit](./setshrinktofit/) | Represents if text automatically shrinks to fit in the available column width. |
|[GetTextDirection](./gettextdirection/) | Represents text reading order. |
|[SetTextDirection](./settextdirection/) | Represents text reading order. |
|[IsJustifyDistributed](./isjustifydistributed/) | Indicates if the cells justified or distributed alignment should be used on the last line of text. |
|[SetIsJustifyDistributed](./setisjustifydistributed/) | Indicates if the cells justified or distributed alignment should be used on the last line of text. |
|[GetQuotePrefix](./getquoteprefix/) | Indicates whether the cell's value starts with single quote mark. |
|[SetQuotePrefix](./setquoteprefix/) | Indicates whether the cell's value starts with single quote mark. |
|[IsGradient](./isgradient/) | Indicates whether the cell shading is a gradient pattern. |
|[SetIsGradient](./setisgradient/) | Indicates whether the cell shading is a gradient pattern. |
|[SetTwoColorGradient](./settwocolorgradient/) | Sets the specified fill to a two-color gradient. |
|[GetTwoColorGradientSetting](./gettwocolorgradientsetting/) | Get the two-color gradient setting. |
|[IsPercent](./ispercent/) | Indicates whether the number format is a percent format. |
|[IsDateTime](./isdatetime/) | Indicates whether the number format is a date format. |
|[ToJson](./tojson/) | Convert Style to JSON struct data. |
