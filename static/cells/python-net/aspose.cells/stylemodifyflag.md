##StyleModifyFlag enumeration
## StyleModifyFlag enumeration
The style modified flags.
The StyleModifyFlag type exposes the following members:
### Fields
| Field | Description |
| :- | :- |
| LEFT_BORDER | Indicates whether left border has been modified for the style. |
| RIGHT_BORDER | Indicates whether right border has been modified for the style. |
| TOP_BORDER | Indicates whether top border has been modified for the style. |
| BOTTOM_BORDER | Indicates whether bottom border has been modified for the style. |
| DIAGONAL_DOWN_BORDER | Indicates whether diagonal-down border has been modified for the style. |
| DIAGONAL_UP_BORDER | Indicates whether diagonal-up border has been modified for the style. |
| HORIZONTAL_BORDER | Indicates whether horizontal border has been modified for the style.
| VERTICAL_BORDER | Indicates whether vertical border has been modified for the style.
| SIDE_BORDERS | Indicates the four side borders: [`StyleModifyFlag.LEFT_BORDER`](/cells/python-net/aspose.cells/stylemodifyflag#LEFT_BORDER),
| DIAGONAL | Indicates diagonal borders: [`StyleModifyFlag.DIAGONAL_DOWN_BORDER`](/cells/python-net/aspose.cells/stylemodifyflag#DIAGONAL_DOWN_BORDER) and [`StyleModifyFlag.DIAGONAL_UP_BORDER`](/cells/python-net/aspose.cells/stylemodifyflag#DIAGONAL_UP_BORDER). |
| DYNAMIC_STYLE_BORDERS | Indicates borders of dynamic style: [`StyleModifyFlag.HORIZONTAL_BORDER`](/cells/python-net/aspose.cells/stylemodifyflag#HORIZONTAL_BORDER) and [`StyleModifyFlag.VERTICAL_BORDER`](/cells/python-net/aspose.cells/stylemodifyflag#VERTICAL_BORDER). |
| BORDERS | Indicates whether one or more borders([`StyleModifyFlag.LEFT_BORDER`](/cells/python-net/aspose.cells/stylemodifyflag#LEFT_BORDER),
| NUMBER_FORMAT | Indicates whether numberformat has been modified. |
| HORIZONTAL_ALIGNMENT | Indicates whether horizontal alignment has been modified. |
| VERTICAL_ALIGNMENT | Indicates whether vertical alignment has been modified. |
| INDENT | Indicates whether indent property has been modified. |
| ROTATION | Indicates whether rotation property has been modified. |
| WRAP_TEXT | Indicates whether wrap text property has been modified. |
| SHRINK_TO_FIT | Indicates whether shrink to fit property has been modified. |
| TEXT_DIRECTION | Indicates whether text direction property has been modified. |
| RELATIVE_INDENT | Indicates whether relative indent property has been modified for the style.
| ALIGNMENT_SETTINGS | Indicates whether one or more alignment-related properties([`StyleModifyFlag.HORIZONTAL_ALIGNMENT`](/cells/python-net/aspose.cells/stylemodifyflag#HORIZONTAL_ALIGNMENT),
| PATTERN | Indicates whether pattern of the shading has been modified. |
| FOREGROUND_COLOR | Indicates whether foreground color has been modified. |
| BACKGROUND_COLOR | Indicates whether background color has been modified. |
| CELL_SHADING | Indicates whether one or more shading-related properties([`StyleModifyFlag.PATTERN`](/cells/python-net/aspose.cells/stylemodifyflag#PATTERN),
| LOCKED | Indicates whether locked property has been modified. |
| HIDE_FORMULA | Indicates whether hide formula has been modified. |
| PROTECTION_SETTINGS | Indicates whether one or more protection-related properties([`StyleModifyFlag.LOCKED`](/cells/python-net/aspose.cells/stylemodifyflag#LOCKED),
| FONT_SIZE | Indicates whether font size has been modified. |
| FONT_NAME | Indicates whether font name has been modified. |
| FONT_COLOR | Indicates whether font color has been modified. |
| FONT_WEIGHT | Indicates whether font weight has been modified. |
| FONT_ITALIC | Indicates whether italic property of font has been modified. |
| FONT_UNDERLINE | Indicates whether underline property of font has been modified. |
| FONT_STRIKE | Indicates whether strike property font has been modified. |
| FONT_SCRIPT | Indicates whether subscript or superscript property of font has been modified. |
| FONT_FAMILY | Indicates whether font family has been modified. |
| FONT_CHARSET | Indicates whether charset of the font has been modified. |
| FONT_SCHEME | unused. |
| FONT_DIRTY | unused. |
| FONT_SPELLING_ERROR | unused. |
| FONT_U_FILL_TX | unused. |
| FONT_SPACING | unused. |
| FONT_KERNING | unused. |
| FONT_EQUALIZE | unused. |
| FONT_CAP | unused. |
| FONT_VERTICAL_TEXT |  |
| FONT | Indicates whether one or more properties have been modified for the font of the style. |
| ALL | All properties that can be modified for the style. |
| NONE | No property has been specified. |
### Remarks
Combinations of multiple properties are defined for user's convenience.
When checking whether they are modified for one style, the returned value denotes
whether one or more properties in the combination have been modified.
### See Also
* module [`aspose.cells`](..)
