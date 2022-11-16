---
title: Style
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 1390
url: /python-net/aspose.cells/style/
---

## Style class

Represents display style of excel document,such as font,color,alignment,border,etc.<br/>            The Style object contains all style attributes (font, number format, alignment, and so on) as properties.

The Style type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|Style()|Initializes a new instance of the [Style](/cells/python-net/aspose.cells/style/) class.|
## Properties
| Name | Description |
| :- | :- |
|background_theme_color|Gets and sets the background theme color.|
|foreground_theme_color|Gets and sets the foreground theme color.|
|name|Gets or sets the name of the style.|
|pattern|Gets or sets the cell background pattern type.|
|borders|Gets the [BorderCollection](/cells/python-net/aspose.cells/bordercollection/) of the style.|
|background_color|Gets or sets a style's background color.|
|background_argb_color|Gets and sets the background color with a 32-bit ARGB value.|
|foreground_color|Gets or sets a style's foreground color.|
|foreground_argb_color|Gets and sets the foreground color with a 32-bit ARGB value.|
|has_borders|Checks whether there are borders have been set for the style.|
|parent_style|Gets the parent style of this style.|
|indent_level|Represents the indent level for the cell or range. Can only be an integer from 0 to 250.|
|font|Gets a [font](/cells/python-net/aspose.cells/style/) object.|
|rotation_angle|Represents text rotation angle.|
|horizontal_alignment|Gets or sets the horizontal alignment type of the text in a cell.|
|vertical_alignment|Gets or sets the vertical alignment type of the text in a cell.|
|is_text_wrapped|Gets or sets a value indicating whether the text within a cell is wrapped.|
|number|Gets or sets the display format of numbers and dates. The formatting patterns are different for different regions.|
|is_locked|Gets or sets a value indicating whether a cell can be modified or not.|
|custom|Represents the custom number format string of this style object.<br/>            If the custom number format is not set(For example, the number format is builtin), "" will be returned.|
|culture_custom|Gets and sets the culture-dependent pattern string for number format.<br/>            If no number format has been set for this object, null will be returned.<br/>            If number format is builtin, the pattern string corresponding to the builtin number will be returned.|
|invariant_custom|Gets the culture-independent pattern string for number format.<br/>            If no number format has been set for this object, null will be returned.<br/>            If number format is builtin, the pattern string corresponding to the builtin number will be returned.|
|is_formula_hidden|Represents if the formula will be hidden when the worksheet is protected.|
|shrink_to_fit|Represents if text automatically shrinks to fit in the available column width.|
|text_direction|Represents text reading order.|
|is_justify_distributed|Indicates if the cells justified or distributed alignment should be used on the last line of text.|
|quote_prefix|Indicates whether the cell's value starts with single quote mark.|
|is_gradient|Indicates whether the cell shading is a gradient pattern.|
|is_percent|Indicates whether the number format is a percent format.|
|is_date_time|Indicates whether the number format is a date format.|
## Methods
| Name | Description |
| :- | :- |
|set_border(border_type, border_style, border_color)|Sets the borders of the style.|
|set_border(border_type, border_style, border_color)|Sets the borders of the style.|
|set_pattern_color(pattern, color1, color2)|Sets the background color.|
|copy(style)|Copies data from another style object|
|update()|Apply the named style to the styles of the cells which use this named style.<br/>            It works like clicking the "ok" button after you finished modifying the style.<br/>            Only applies for named style.|
|is_modified(modify_flag)|Checks whether the specified properties of the style have been modified.<br/>            Used for style of ConditionalFormattings to check whether the specified properties of this style should be used when applying the ConditionalFormattings on a cell.|
|set_custom(custom, builtin_preference)|Sets the Custom number format string of a cell.|
|set_two_color_gradient(color1, color2, gradient_style_type, variant)|Sets the specified fill to a two-color gradient.|
|get_two_color_gradient(color1, color2, gradient_style_type, variant)|Get the two-color gradient setting.|

### See Also

* namespace [aspose.cells](/cells/python-net/aspose.cells/)
* assembly [Aspose.Cells](/cells/python-net/)

