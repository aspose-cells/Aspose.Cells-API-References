---
title: Style klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 1390
url: /sv/python-net/aspose.cells/style/
is_root: false
---
##  Style klass
Representerar visningsstil för Excel-dokument, som typsnitt, färg, justering, kant, etc.
Objektet Style innehåller alla stilattribut (teckensnitt, talformat, justering och så vidare) som egenskaper.



Typen Style avslöjar följande medlemmar:

###  Konstruktörer
| Konstruktör| Beskrivning|
| :- | :- |
| [Style()](/cells/sv/python-net/aspose.cells/style/__init__/#) | Initierar en ny instans av klassen [Style](/cells/sv/python-net/aspose.cells/style).|


###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [background_theme_color](/cells/sv/python-net/aspose.cells/style/background_theme_color) | Hämtar och ställer in bakgrundstemafärgen.|
| [foreground_theme_color](/cells/sv/python-net/aspose.cells/style/foreground_theme_color) | Hämtar och ställer in förgrundstemafärgen.|
| [name](/cells/sv/python-net/aspose.cells/style/name) | Hämtar eller ställer in namnet på stilen.|
| [pattern](/cells/sv/python-net/aspose.cells/style/pattern) | Hämtar eller ställer in cellbakgrundsmönstertypen.|
| [borders](/cells/sv/python-net/aspose.cells/style/borders) | Får stilens [BorderCollection](/cells/sv/python-net/aspose.cells/bordercollection).|
| [background_color](/cells/sv/python-net/aspose.cells/style/background_color) | Hämtar eller ställer in en stils bakgrundsfärg.|
| [background_argb_color](/cells/sv/python-net/aspose.cells/style/background_argb_color) | Hämtar och ställer in bakgrundsfärgen med ett 32-bitars ARGB-värde.|
| [foreground_color](/cells/sv/python-net/aspose.cells/style/foreground_color) | Hämtar eller ställer in en stils förgrundsfärg.|
| [foreground_argb_color](/cells/sv/python-net/aspose.cells/style/foreground_argb_color) | Hämtar och ställer in förgrundsfärgen med ett 32-bitars ARGB-värde.|
| [has_borders](/cells/sv/python-net/aspose.cells/style/has_borders) | Kontrollerar om det finns gränser har satts för stilen.|
| [parent_style](/cells/sv/python-net/aspose.cells/style/parent_style) | Får moderstilen för denna stil.|
| [indent_level](/cells/sv/python-net/aspose.cells/style/indent_level) | Representerar indragsnivån för cellen eller området. Kan bara vara ett heltal från 0 till 250.|
| [font](/cells/sv/python-net/aspose.cells/style/font) | Får ett [Style.font](/cells/sv/python-net/aspose.cells/style#font) objekt.|
| [rotation_angle](/cells/sv/python-net/aspose.cells/style/rotation_angle) | Representerar textrotationsvinkel.|
| [horizontal_alignment](/cells/sv/python-net/aspose.cells/style/horizontal_alignment) | Hämtar eller ställer in den horisontella justeringen av texten i en cell.|
| [vertical_alignment](/cells/sv/python-net/aspose.cells/style/vertical_alignment) | Hämtar eller ställer in den vertikala anpassningstypen för texten i en cell.|
| [is_text_wrapped](/cells/sv/python-net/aspose.cells/style/is_text_wrapped) | Hämtar eller ställer in ett värde som anger om texten i en cell är radbruten.|
| [number](/cells/sv/python-net/aspose.cells/style/number) | Hämtar eller ställer in visningsformat för siffror och datum. Formateringsmönstren är olika för olika regioner.|
| [is_locked](/cells/sv/python-net/aspose.cells/style/is_locked) |Hämtar eller ställer in ett värde som anger om en cell kan ändras eller inte.|
| [custom](/cells/sv/python-net/aspose.cells/style/custom) | Representerar den anpassade nummerformatsträngen för detta stilobjekt.<br/>Om det anpassade sifferformatet inte är inställt (Till exempel, sifferformatet är inbyggt), kommer "" att returneras.|
| [culture_custom](/cells/sv/python-net/aspose.cells/style/culture_custom) | Hämtar och ställer in den kulturberoende mönstersträngen för talformat.<br/>Om inget talformat har ställts in för detta objekt, returneras null.<br/> Om talformat är inbyggt kommer mönstersträngen som motsvarar det inbyggda numret att returneras.|
| [invariant_custom](/cells/sv/python-net/aspose.cells/style/invariant_custom) | Hämtar den kulturoberoende mönstersträngen för talformat.<br/>Om inget talformat har ställts in för detta objekt, returneras null.<br/> Om talformat är inbyggt kommer mönstersträngen som motsvarar det inbyggda numret att returneras.|
| [is_formula_hidden](/cells/sv/python-net/aspose.cells/style/is_formula_hidden) | Representerar om formeln kommer att döljas när kalkylbladet är skyddat.|
| [shrink_to_fit](/cells/sv/python-net/aspose.cells/style/shrink_to_fit) | Representerar om text automatiskt krymper för att passa den tillgängliga kolumnbredden.|
| [text_direction](/cells/sv/python-net/aspose.cells/style/text_direction) | Representerar textläsordning.|
| [is_justify_distributed](/cells/sv/python-net/aspose.cells/style/is_justify_distributed) | Anger om cellerna justerad eller distribuerad justering ska användas på den sista textraden.|
| [quote_prefix](/cells/sv/python-net/aspose.cells/style/quote_prefix) | Anger om cellens värde börjar med enkla citattecken.|
| [is_gradient](/cells/sv/python-net/aspose.cells/style/is_gradient) | Indikerar om cellskuggningen är ett gradientmönster.|
| [is_percent](/cells/sv/python-net/aspose.cells/style/is_percent) | Anger om talformatet är ett procentformat.|
| [is_date_time](/cells/sv/python-net/aspose.cells/style/is_date_time) | Anger om sifferformatet är ett datumformat.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [set_border(border_type, border_style, border_color)](/cells/sv/python-net/aspose.cells/style/set_border/#BorderType-CellBorderType-aspose.pydrawing.Color) | Ställer in gränserna för stilen.|
| [set_border(border_type, border_style, border_color)](/cells/sv/python-net/aspose.cells/style/set_border/#BorderType-CellBorderType-CellsColor) | Ställer in gränserna för stilen.|
| [set_pattern_color(pattern, color1, color2)](/cells/sv/python-net/aspose.cells/style/set_pattern_color/#BackgroundType-aspose.pydrawing.Color-aspose.pydrawing.Color) | Ställer in bakgrundsfärgen.|
| [copy(style)](/cells/sv/python-net/aspose.cells/style/copy/#Style) | Kopierar data från ett annat stilobjekt|
| [update()](/cells/sv/python-net/aspose.cells/style/update/#) | Tillämpa den namngivna stilen på stilarna i cellerna som använder denna namngivna stil.<br/>Det fungerar som att klicka på "ok"-knappen efter att du har ändrat stilen.<br/> Gäller endast namngiven stil.|
| [is_modified(modify_flag)](/cells/sv/python-net/aspose.cells/style/is_modified/#StyleModifyFlag) | Kontrollerar om stilens angivna egenskaper har ändrats.<br/> Används för stil för ConditionalFormattings för att kontrollera om de angivna egenskaperna för denna stil ska användas när de ConditionalFormattings tillämpas på en cell.|
| [set_custom(custom, builtin_preference)](/cells/sv/python-net/aspose.cells/style/set_custom/#str-bool) | Ställer in den anpassade nummerformatsträngen för en cell.|
| [set_two_color_gradient(color1, color2, gradient_style_type, variant)](/cells/sv/python-net/aspose.cells/style/set_two_color_gradient/#aspose.pydrawing.Color-aspose.pydrawing.Color-aspose.cells.drawing.GradientStyleType-int) | Ställer in den angivna fyllningen till en tvåfärgsgradient.|
| [get_two_color_gradient(color1, color2, gradient_style_type, variant)](/cells/sv/python-net/aspose.cells/style/get_two_color_gradient/#aspose.pydrawing.Color&-aspose.pydrawing.Color&-any-any) | Få inställningen för tvåfärgsgradient.|
| [get_two_color_gradient_setting()](/cells/sv/python-net/aspose.cells/style/get_two_color_gradient_setting/#) | Få inställningen för tvåfärgsgradient.|
| [to_json()](/cells/sv/python-net/aspose.cells/style/to_json/#) | Konvertera [Style](/cells/sv/python-net/aspose.cells/style) till JSON strukturdata.|



###  Exempel

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

###  Se även
* modul [aspose.cells](..)
* klass [BorderCollection](/cells/sv/python-net/aspose.cells/bordercollection)
* klass [Style](/cells/sv/python-net/aspose.cells/style)
