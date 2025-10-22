##NaryEquationNode class
## NaryEquationNode class
This class specifies an n-ary operator equation consisting of an n-ary operator, a base (or operand), and optional upper and lower bounds.
**Inheritance:** [`NaryEquationNode`](/cells/python-net/aspose.cells.drawing.equations/naryequationnode)
The NaryEquationNode type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [type](/cells/python-net/aspose.cells.drawing.equations/naryequationnode/type) |  |
| [start_index](/cells/python-net/aspose.cells.drawing.equations/naryequationnode/start_index) |  |
| [length](/cells/python-net/aspose.cells.drawing.equations/naryequationnode/length) |  |
| [font](/cells/python-net/aspose.cells.drawing.equations/naryequationnode/font) |  |
| [text_options](/cells/python-net/aspose.cells.drawing.equations/naryequationnode/text_options) |  |
| [parent_node](/cells/python-net/aspose.cells.drawing.equations/naryequationnode/parent_node) |  |
| [equation_type](/cells/python-net/aspose.cells.drawing.equations/naryequationnode/equation_type) |  |
| [is_hide_subscript](/cells/python-net/aspose.cells.drawing.equations/naryequationnode/is_hide_subscript) | Whether to display the lower bound |
| [is_hide_superscript](/cells/python-net/aspose.cells.drawing.equations/naryequationnode/is_hide_superscript) | Whether to display the upper bound |
| [limit_location](/cells/python-net/aspose.cells.drawing.equations/naryequationnode/limit_location) | This attribute specifies the location of limits in n-ary operators. Limits can be either centered above and below the n-ary operator, or positioned just to the right of the operator. |
| [nary_operator](/cells/python-net/aspose.cells.drawing.equations/naryequationnode/nary_operator) | an n-ary operator.e.g "∑".
| [nary_operator_type](/cells/python-net/aspose.cells.drawing.equations/naryequationnode/nary_operator_type) | an n-ary operator.e.g "∑" |
| [nary_grow](/cells/python-net/aspose.cells.drawing.equations/naryequationnode/nary_grow) | This attribute specifies the growth property of n-ary operators at the document level. When off, n-ary operators such as integrals and summations do not grow to match the size of their operand height. When on, the n-ary operator grows vertically to match its operand height. |
### Methods
| Method | Description |
| :- | :- |
| [`add_child(self, equation_type)`](/cells/python-net/aspose.cells.drawing.equations/naryequationnode/add_child/#aspose.cells.drawing.equations.equationnodetype) |  |
| [`add_child(self, node)`](/cells/python-net/aspose.cells.drawing.equations/naryequationnode/add_child/#aspose.cells.drawing.equations.equationnode) |  |
| [`remove_child(self, node)`](/cells/python-net/aspose.cells.drawing.equations/naryequationnode/remove_child/#aspose.cells.drawing.equations.equationnode) |  |
| [`remove_child(self, index)`](/cells/python-net/aspose.cells.drawing.equations/naryequationnode/remove_child/#int) |  |
| [`set_word_art_style(self, style)`](/cells/python-net/aspose.cells.drawing.equations/naryequationnode/set_word_art_style/#aspose.cells.drawing.presetwordartstyle) |  |
| [`to_la_te_x(self)`](/cells/python-net/aspose.cells.drawing.equations/naryequationnode/to_la_te_x/#) |  |
| [`to_math_ml(self)`](/cells/python-net/aspose.cells.drawing.equations/naryequationnode/to_math_ml/#) |  |
| [`insert_child(self, index, equation_type)`](/cells/python-net/aspose.cells.drawing.equations/naryequationnode/insert_child/#int-aspose.cells.drawing.equations.equationnodetype) |  |
| [`insert_after(self, equation_type)`](/cells/python-net/aspose.cells.drawing.equations/naryequationnode/insert_after/#aspose.cells.drawing.equations.equationnodetype) |  |
| [`insert_before(self, equation_type)`](/cells/python-net/aspose.cells.drawing.equations/naryequationnode/insert_before/#aspose.cells.drawing.equations.equationnodetype) |  |
| [`get_child(self, index)`](/cells/python-net/aspose.cells.drawing.equations/naryequationnode/get_child/#int) |  |
| [`remove(self)`](/cells/python-net/aspose.cells.drawing.equations/naryequationnode/remove/#) |  |
| [`remove_all_children(self)`](/cells/python-net/aspose.cells.drawing.equations/naryequationnode/remove_all_children/#) |  |
| [`create_node(, equation_type, workbook, parent)`](/cells/python-net/aspose.cells.drawing.equations/naryequationnode/create_node/#aspose.cells.drawing.equations.equationnodetype-aspose.cells.workbook-aspose.cells.drawing.equations.equationnode) |  |
### See Also
* module [`aspose.cells.drawing.equations`](..)
* class [`NaryEquationNode`](/cells/python-net/aspose.cells.drawing.equations/naryequationnode)
