---
title: Style clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 1390
url: /es/python-net/aspose.cells/style/
is_root: false
---
##  Style clase
Representa el estilo de visualización del documento de Excel, como fuente, color, alineación, borde, etc.
El objeto Style contiene todos los atributos de estilo (fuente, formato de número, alineación, etc.) como propiedades.



El tipo Style expone los siguientes miembros:

###  Constructores
| Constructor| Descripción|
| :- | :- |
| [Style()](/cells/es/python-net/aspose.cells/style/__init__/#) | Inicializa una nueva instancia de la clase [Style](/cells/es/python-net/aspose.cells/style).|


###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [background_theme_color](/cells/es/python-net/aspose.cells/style/background_theme_color) | Obtiene y establece el color del tema de fondo.|
| [foreground_theme_color](/cells/es/python-net/aspose.cells/style/foreground_theme_color) | Obtiene y establece el color del tema de primer plano.|
| [name](/cells/es/python-net/aspose.cells/style/name) | Obtiene o establece el nombre del estilo.|
| [pattern](/cells/es/python-net/aspose.cells/style/pattern) | Obtiene o establece el tipo de patrón de fondo de la celda.|
| [borders](/cells/es/python-net/aspose.cells/style/borders) | Obtiene el [BorderCollection](/cells/es/python-net/aspose.cells/bordercollection) del estilo.|
| [background_color](/cells/es/python-net/aspose.cells/style/background_color) | Obtiene o establece el color de fondo de un estilo.|
| [background_argb_color](/cells/es/python-net/aspose.cells/style/background_argb_color) | Obtiene y establece el color de fondo con un valor ARGB de 32 bits.|
| [foreground_color](/cells/es/python-net/aspose.cells/style/foreground_color) | Obtiene o establece el color de primer plano de un estilo.|
| [foreground_argb_color](/cells/es/python-net/aspose.cells/style/foreground_argb_color) | Obtiene y establece el color de primer plano con un valor ARGB de 32 bits.|
| [has_borders](/cells/es/python-net/aspose.cells/style/has_borders) | Comprueba si se han establecido bordes para el estilo.|
| [parent_style](/cells/es/python-net/aspose.cells/style/parent_style) | Obtiene el estilo principal de este estilo.|
| [indent_level](/cells/es/python-net/aspose.cells/style/indent_level) | Representa el nivel de sangría de la celda o rango. Solo puede ser un número entero de 0 a 250.|
| [font](/cells/es/python-net/aspose.cells/style/font) | Obtiene un objeto [Style.font](/cells/es/python-net/aspose.cells/style#font).|
| [rotation_angle](/cells/es/python-net/aspose.cells/style/rotation_angle) | Representa el ángulo de rotación del texto.|
| [horizontal_alignment](/cells/es/python-net/aspose.cells/style/horizontal_alignment) | Obtiene o establece el tipo de alineación horizontal del texto de una celda.|
| [vertical_alignment](/cells/es/python-net/aspose.cells/style/vertical_alignment) | Obtiene o establece el tipo de alineación vertical del texto de una celda.|
| [is_text_wrapped](/cells/es/python-net/aspose.cells/style/is_text_wrapped) | Obtiene o establece un valor que indica si el texto de una celda está ajustado.|
| [number](/cells/es/python-net/aspose.cells/style/number) | Obtiene o establece el formato de visualización de números y fechas. Los patrones de formato son diferentes para las diferentes regiones.|
| [is_locked](/cells/es/python-net/aspose.cells/style/is_locked) |Obtiene o establece un valor que indica si una celda se puede modificar o no.|
| [custom](/cells/es/python-net/aspose.cells/style/custom) | Representa la cadena de formato de número personalizado de este objeto de estilo.<br/>Si el formato de número personalizado no está configurado (por ejemplo, el formato de número está integrado), se devolverá "".|
| [culture_custom](/cells/es/python-net/aspose.cells/style/culture_custom) | Obtiene y establece la cadena de patrón dependiente de la referencia cultural para el formato de número.<br/>Si no se ha establecido un formato de número para este objeto, se devolverá un valor nulo.<br/> Si el formato de número está integrado, se devolverá la cadena de patrón correspondiente al número integrado.|
| [invariant_custom](/cells/es/python-net/aspose.cells/style/invariant_custom) | Obtiene la cadena de patrón independiente de la referencia cultural para el formato de número.<br/>Si no se ha establecido un formato de número para este objeto, se devolverá un valor nulo.<br/> Si el formato de número está integrado, se devolverá la cadena de patrón correspondiente al número integrado.|
| [is_formula_hidden](/cells/es/python-net/aspose.cells/style/is_formula_hidden) | Representa si la fórmula se ocultará cuando la hoja de cálculo esté protegida.|
| [shrink_to_fit](/cells/es/python-net/aspose.cells/style/shrink_to_fit) | Representa si el texto se reduce automáticamente para ajustarse al ancho de columna disponible.|
| [text_direction](/cells/es/python-net/aspose.cells/style/text_direction) | Representa el orden de lectura del texto.|
| [is_justify_distributed](/cells/es/python-net/aspose.cells/style/is_justify_distributed) | Indica si en la última línea de texto se debe utilizar la alineación justificada o distribuida de las celdas.|
| [quote_prefix](/cells/es/python-net/aspose.cells/style/quote_prefix) | Indica si el valor de la celda comienza con comillas simples.|
| [is_gradient](/cells/es/python-net/aspose.cells/style/is_gradient) | Indica si el sombreado de la celda es un patrón de degradado.|
| [is_percent](/cells/es/python-net/aspose.cells/style/is_percent) | Indica si el formato de número es un formato de porcentaje.|
| [is_date_time](/cells/es/python-net/aspose.cells/style/is_date_time) | Indica si el formato de número es un formato de fecha.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [set_border(border_type, border_style, border_color)](/cells/es/python-net/aspose.cells/style/set_border/#BorderType-CellBorderType-aspose.pydrawing.Color) | Establece los bordes del estilo.|
| [set_border(border_type, border_style, border_color)](/cells/es/python-net/aspose.cells/style/set_border/#BorderType-CellBorderType-CellsColor) | Establece los bordes del estilo.|
| [set_pattern_color(pattern, color1, color2)](/cells/es/python-net/aspose.cells/style/set_pattern_color/#BackgroundType-aspose.pydrawing.Color-aspose.pydrawing.Color) | Establece el color de fondo.|
| [copy(style)](/cells/es/python-net/aspose.cells/style/copy/#Style) | Copia datos de otro objeto de estilo|
| [update()](/cells/es/python-net/aspose.cells/style/update/#) | Aplique el estilo con nombre a los estilos de las celdas que usan este estilo con nombre.<br/>Funciona como hacer clic en el botón "Aceptar" después de terminar de modificar el estilo.<br/> Solo se aplica al estilo con nombre.|
| [is_modified(modify_flag)](/cells/es/python-net/aspose.cells/style/is_modified/#StyleModifyFlag) | Comprueba si se han modificado las propiedades especificadas del estilo.<br/> Se usa para el estilo de ConditionalFormattings para verificar si las propiedades especificadas de este estilo deben usarse al aplicar ConditionalFormattings en una celda.|
| [set_custom(custom, builtin_preference)](/cells/es/python-net/aspose.cells/style/set_custom/#str-bool) | Establece la cadena de formato de número personalizado de una celda.|
| [set_two_color_gradient(color1, color2, gradient_style_type, variant)](/cells/es/python-net/aspose.cells/style/set_two_color_gradient/#aspose.pydrawing.Color-aspose.pydrawing.Color-aspose.cells.drawing.GradientStyleType-int) | Establece el relleno especificado en un degradado de dos colores.|
| [get_two_color_gradient(color1, color2, gradient_style_type, variant)](/cells/es/python-net/aspose.cells/style/get_two_color_gradient/#aspose.pydrawing.Color&-aspose.pydrawing.Color&-any-any) | Obtenga la configuración de degradado de dos colores.|
| [get_two_color_gradient_setting()](/cells/es/python-net/aspose.cells/style/get_two_color_gradient_setting/#) | Obtenga la configuración de degradado de dos colores.|
| [to_json()](/cells/es/python-net/aspose.cells/style/to_json/#) | Convierta [Style](/cells/es/python-net/aspose.cells/style) a JSON datos de estructura.|



###  Ejemplo

```python
from aspose.cells import Workbook
from aspose.pydrawing import Color

workbook = Workbook()
sheets = workbook.worksheets
cell = sheets[0].cells.get("A1")
style = cell.get_style()
style.font.name = "Times New Roman"
style.font.color = Color.blue
cell.set_style(style)

```

###  Ver también
* módulo [aspose.cells](..)
* clase [BorderCollection](/cells/es/python-net/aspose.cells/bordercollection)
* clase [Style](/cells/es/python-net/aspose.cells/style)
