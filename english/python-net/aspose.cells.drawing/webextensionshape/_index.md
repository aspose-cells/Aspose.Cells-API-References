---
title: WebExtensionShape
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 750
url: /cells/python-net/aspose.cells.drawing/webextensionshape/
---

## WebExtensionShape class

Represents the shape of web extension.

The WebExtensionShape type exposes the following members:
## Properties
| Name | Description |
| :- | :- |
|macro_name|Gets and sets the name of macro.|
|is_equation|Indicates whether the shape only contains an equation.|
|is_smart_art|Indicates whether the shape is smart art.|
|z_order_position|Returns the position of a shape in the z-order.|
|name|Gets and sets the name of the shape.|
|alternative_text|Returns or sets the descriptive (alternative) text string of the [Shape](/cells/python-net/aspose.cells.drawing/shape/) object.|
|title|Specifies the title (caption) of the current shape object.|
|line_format|Returns a MsoLineFormat object that contains line formatting properties for the specified shape.|
|fill_format|Returns a MsoFillFormat object that contains fill formatting properties for the specified shape.|
|format|Represents the setting of the shape's formatting.|
|line|Gets line style|
|fill|Returns a [fill_format](/cells/python-net/aspose.cells.drawing/shape/) object that contains fill formatting properties for the specified shape.|
|shadow_effect|Represents a|
|reflection|Represents a|
|glow|Represents a|
|soft_edges|Gets and sets the radius of blur to apply to the edges, in unit of points.|
|three_d_format|Gets and sets 3d format of the shape.|
|text_frame|Returns a TextFrame object that contains the alignment and anchoring properties for the specified shape.|
|format_picture|Gets and sets the options of the picture format.|
|is_hidden|Indicates whether the object is visible.|
|is_lock_aspect_ratio|True means that don't allow changes in aspect ratio.|
|rotation_angle|Gets and sets the rotation of the shape.|
|hyperlink|Gets the hyperlink of the shape.|
|id|Gets the identifier of this shape.|
|spid|Specifies an optional string that an application can use to Identify the particular shape.|
|spt|Specifies an optional number that an application can use to associate the particular shape with a defined shape type.|
|worksheet|Gets the [worksheet](/cells/python-net/aspose.cells.drawing/shape/) object which contains this shape.|
|is_group|Indicates whether the shape is a group.|
|is_in_group|Indicates whether the shape is grouped.|
|is_word_art|Indicates whether this shape is a word art.|
|text_effect|Returns a TextEffectFormat object that contains text-effect formatting properties for the specified shape. <br/>            Applies to Shape objects that represent WordArt.|
|is_locked|True if the object is locked, False if the object can be modified when the sheet is protected.|
|is_printable|True if the object is printable|
|mso_drawing_type|Gets mso drawing type.|
|auto_shape_type|Gets and sets the auto shape type.|
|anchor_type|Gets and set the shape anchor placeholder.|
|placement|Represents the way the drawing object is attached to the cells below it.<br/>            The property controls the placement of an object on a worksheet.|
|upper_left_row|Represents upper left corner row index.|
|upper_delta_y|Gets or sets the shape's vertical offset from its upper left corner row.|
|upper_left_column|Represents upper left corner column index.|
|upper_delta_x|Gets or sets the shape's horizontal offset from its upper left corner column.|
|lower_right_row|Represents lower right corner row index.|
|lower_delta_y|Gets or sets the shape's vertical offset from its lower right corner row.|
|lower_right_column|Represents lower right corner column index.|
|lower_delta_x|Gets or sets the shape's horizontal  offset from its lower right corner column.|
|right|Represents the width of the shape's horizontal  offset from its lower right corner column, in unit of pixels.|
|bottom|Represents the width of the shape's vertical offset from its lower bottom corner row, in unit of pixels.|
|width|Represents the width of shape, in unit of pixels.|
|width_inch|Represents the width of the shape, in unit of inch.|
|width_pt|Represents the width of the shape, in unit of point.|
|width_cm|Represents the width of the shape, in unit of centimeters.|
|height|Represents the height of shape, in unit of pixel.|
|height_inch|Represents the height of the shape, in unit of inches.|
|height_pt|Represents the height of the shape, in unit of points.|
|height_cm|Represents the height of the shape, in unit of centimeters.|
|left|Represents the horizontal offset of shape from its left column, in unit of pixels.|
|left_inch|Represents the horizontal offset of shape from its left column, in unit of inches.|
|left_cm|Represents the horizontal offset of shape from its left column, in unit of centimeters.|
|top|Represents the vertical offset of shape from its top row, in unit of pixels.|
|top_inch|Represents the vertical offset of shape from its top row, in unit of inches.|
|top_cm|Represents the vertical offset of shape from its top row, in unit of centimeters.|
|top_to_corner|Gets and sets the vertical offset of shape from worksheet top border, in unit of pixels.|
|left_to_corner|Gets and sets the horizonal offset of shape from worksheet left border.|
|x|Gets and sets the horizontal offset of shape from worksheet left border,in unit of pixels.|
|y|Gets and sets the vertical offset of shape from worksheet top border,in unit of pixels.|
|width_scale|Gets and sets the width scale, in unit of percent of the original picture width.<br/>            If the shape is not picture ,the WidthScale property only returns 100;|
|height_scale|Gets and sets the height scale,in unit of percent of the original picture height.<br/>            If the shape is not picture ,the HeightScale property only returns 100;|
|top_in_shape|Represents the vertical offset of shape from the top border of the parent shape, <br/>            in unit of 1/4000 of height of the parent shape.|
|left_in_shape|Represents the horizontal offset of shape from the left border of the parent shape, <br/>            in unit of 1/4000 of width of the parent shape.|
|width_in_shape|Represents the width of the shape, in unit of 1/4000 of the parent shape.|
|height_in_shape|Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape..|
|group|Gets the group shape which contains this shape.|
|type|Gets the auto shape type.|
|has_line|Gets and sets the line border of the shape is visible.|
|is_filled|Indicates whether the fill format is visible.|
|is_flipped_horizontally|Gets and sets whether shape is horizontally flipped .|
|is_flipped_vertically|Gets and sets whether shape is vertically flipped .|
|actual_lower_right_row|Get the actual bottom row.|
|connection_points|Get the connection points|
|relative_to_original_picture_size|Indicates whether shape is relative to original picture size.|
|linked_cell|Gets or sets the worksheet range linked to the control's value.|
|input_range|Gets or sets the worksheet range used to fill the specified combo box.|
|text_shape_type|Gets and sets the preset text shape type.|
|text_body|Gets and sets the setting of the shape's text.|
|font|Represents the font of shape.|
|text_options|Represents the text options of the shape.|
|text|Represents the string in this TextBox object.|
|is_rich_text|Whether or not the text is rich text.|
|html_text|Gets and sets the html string which contains data and some formats in this textbox.|
|text_vertical_overflow|Gets and sets the text vertical overflow type of the shape which contains text.|
|text_horizontal_overflow|Gets and sets the text horizontal overflow type of the shape which contains text.|
|is_text_wrapped|Gets and sets the text wrapped type of the shape which contains text.|
|text_orientation_type|Gets and sets the text orientation type of the shape.|
|text_horizontal_alignment|Gets and sets the text horizontal alignment type of the shape.|
|text_vertical_alignment|Gets and sets the text vertical alignment type of the shape.|
|text_direction|Gets/Sets the direction of the text flow for this object.|
|control_data|Gets the data of control.|
|active_x_control|Gets the ActiveX control.|
|paths|Gets the paths of a custom geometric shape.|
|geometry|Gets the geometry|
|create_id|Gets and sets create id for this shape.|
|web_extension|Gets and set the web extension.|
## Methods
| Name | Description |
| :- | :- |
|to_image(stream, image_type)|Creates the shape image and saves it to a stream in the specified format.|
|to_image(image_file, options)|Saves the shape to a file.|
|to_image(stream, options)|Saves the shape to a stream.|
|format_characters(start_index, length, font, flag)|Formats some characters with the font setting.|
|format_characters(start_index, length, font)|Formats some characters with the font setting.|
|get_result_of_smart_art()|Converting smart art to grouped shapes.|
|to_front_or_back(orders)|Brings the shape to the front or sends the shape to back.|
|get_locked_property(type)|Gets the value of locked property.|
|set_locked_property(type, value)|Set the locked property.|
|add_hyperlink(address)|Adds a hyperlink to the shape.|
|remove_hyperlink()|Remove the hyperlink of the shape.|
|move_to_range(upper_left_row, upper_left_column, lower_right_row, lower_right_column)|Moves the shape to a specified range.|
|align_top_right_corner(top_row, right_column)|Moves the picture to the top-right corner.|
|get_connection_points()|Get the connection points|
|get_linked_cell(is_r1c1, is_local)|Gets the range linked to the control's value.|
|set_linked_cell(formula, is_r1c1, is_local)|Sets the range linked to the control's value.|
|get_input_range(is_r1c1, is_local)|Gets the range used to fill the control.|
|set_input_range(formula, is_r1c1, is_local)|Sets the range used to fill the control.|
|update_selected_value()|Update the selected value by the value of the linked cell.|
|calculate_text_size()|Recalculate the text area|
|characters(start_index, length)|Returns a Characters object that represents a range of characters within the text.|
|get_characters()|Returns all Characters objects <br/>            that represents a range of characters within the text .|
|remove_active_x_control()|Remove activeX control.|
|is_same_setting(obj)|Returns whether the shape is same.|

### See Also

* namespace [aspose.cells.drawing](/cells/python-net/aspose.cells.drawing/)
* assembly [Aspose.Cells](/cells/python-net/)

