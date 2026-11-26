---
title: "Clase GridCell"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.GridDesktop.Data.GridCell. Representa un objeto celda"
type: docs
url: /es/net/aspose.cells.griddesktop.data/gridcell/
---
## GridCell class

Representa un objeto de celda.

```csharp
public class GridCell
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BoolValue](../../aspose.cells.griddesktop.data/gridcell/boolvalue/) { get; } | Obtiene el valor booleano contenido en la celda. |
| [Column](../../aspose.cells.griddesktop.data/gridcell/column/) { get; } | Obtiene el número de columna (basado en cero) de la celda. |
| [DateValue](../../aspose.cells.griddesktop.data/gridcell/datevalue/) { get; } | Obtiene el valor DateTime contenido en la celda. |
| [DisplayStringValue](../../aspose.cells.griddesktop.data/gridcell/displaystringvalue/) { get; } | Obtiene el valor de cadena formateado de esta celda. |
| [DoubleValue](../../aspose.cells.griddesktop.data/gridcell/doublevalue/) { get; } | Obtiene el valor double contenido en la celda. |
| [FloatValue](../../aspose.cells.griddesktop.data/gridcell/floatvalue/) { get; } | Obtiene el valor float contenido en la celda. |
| [Formula](../../aspose.cells.griddesktop.data/gridcell/formula/) { get; set; } | Obtiene o establece una fórmula de la celda. |
| [HasCustomStyle](../../aspose.cells.griddesktop.data/gridcell/hascustomstyle/) { get; } | Indica si esta celda tiene configuraciones de estilo personalizadas (diferentes de la predeterminada heredada de la fila, columna o libro de trabajo correspondiente). |
| [HtmlString](../../aspose.cells.griddesktop.data/gridcell/htmlstring/) { get; set; } | Obtiene y establece la cadena html que contiene datos y algunos formatos en esta celda. |
| [IntValue](../../aspose.cells.griddesktop.data/gridcell/intvalue/) { get; } | Obtiene el valor entero contenido en la celda. |
| [IsStyleSet](../../aspose.cells.griddesktop.data/gridcell/isstyleset/) { get; } | Indica si el estilo de la celda está establecido. Si devuelve false, significa que esta celda tiene un formato de celda predeterminado. |
| [Location](../../aspose.cells.griddesktop.data/gridcell/location/) { get; } |  |
| [Name](../../aspose.cells.griddesktop.data/gridcell/name/) { get; } | Obtiene el nombre de la celda. Por ejemplo: A1, F102. |
| [Protected](../../aspose.cells.griddesktop.data/gridcell/protected/) { get; set; } | Indica si la celda está protegida. Si el valor es "true", el usuario no puede modificar la celda a través de la interfaz de usuario. Este atributo no tiene relación con la propiedad Style.CellLocked y no se guardará en el archivo cuando se exporten los datos de la cuadrícula. El valor predeterminado es "false". |
| [Row](../../aspose.cells.griddesktop.data/gridcell/row/) { get; } | Obtiene el número de fila (basado en cero) de la celda. |
| [StringValue](../../aspose.cells.griddesktop.data/gridcell/stringvalue/) { get; } | Obtiene el valor de cadena contenido en la celda. |
| [Style](../../aspose.cells.griddesktop.data/gridcell/style/) { get; set; } | Obtiene la copia del estilo de la celda. establece el estilo para la celda. |
| [Type](../../aspose.cells.griddesktop.data/gridcell/type/) { get; } | devuelve el tipo de valor de la celda, el significado se puede ver en GridCellValueType.java |
| [Value](../../aspose.cells.griddesktop.data/gridcell/value/) { get; set; } | Obtiene el valor contenido en esta celda. |
| [Worksheet](../../aspose.cells.griddesktop.data/gridcell/worksheet/) { get; } | Obtiene el objeto hoja de cálculo. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [ContainsExternalLink](../../aspose.cells.griddesktop.data/gridcell/containsexternallink/)() | Indica si esta celda contiene un enlace externo. Solo se aplica cuando la celda es una celda de fórmula. |
| [Copy](../../aspose.cells.griddesktop.data/gridcell/copy/)(GridCell) | Copia datos de una celda origen. |
| [CopyStyle](../../aspose.cells.griddesktop.data/gridcell/copystyle/)(Style) | copia el estilo y establece el estilo para la celda |
| override [Equals](../../aspose.cells.griddesktop.data/gridcell/equals/)(object) |  |
| [GetCellArea](../../aspose.cells.griddesktop.data/gridcell/getcellarea/)() |  |
| [GetFont](../../aspose.cells.griddesktop.data/gridcell/getfont/)() | Obtiene la fuente de la celda. Cuando cambie la fuente, debe invocar el método "SetFont", para establecer la fuente en la celda. |
| [GetFontColor](../../aspose.cells.griddesktop.data/gridcell/getfontcolor/)() | Obtiene el color de fuente de la celda. Cuando cambie el color, debe invocar el método "SetFontColor", para establecer el color de fuente en la celda. |
| override [GetHashCode](../../aspose.cells.griddesktop.data/gridcell/gethashcode/)() |  |
| [GetStyle](../../aspose.cells.griddesktop.data/gridcell/getstyle/)() | Obtiene el estilo de la celda. Cuando cambie el estilo, debe invocar el método "SetStyle", para establecer el estilo en la celda. |
| [GetValidation](../../aspose.cells.griddesktop.data/gridcell/getvalidation/)() | Obtiene la validación que se aplica a esta celda. Si no está establecida, devuelve null. |
| [GetWidthOfValue](../../aspose.cells.griddesktop.data/gridcell/getwidthofvalue/)() | Obtiene el ancho del valor en unidades de píxeles. |
| [GetWorksheet](../../aspose.cells.griddesktop.data/gridcell/getworksheet/)() | Obtiene la hoja de cálculo principal. |
| [IsErrorValue](../../aspose.cells.griddesktop.data/gridcell/iserrorvalue/)() | Comprueba si una fórmula puede evaluar correctamente un resultado. |
| [IsFormula](../../aspose.cells.griddesktop.data/gridcell/isformula/)() | Representa si la celda especificada contiene una fórmula. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue)(bool) | Coloca un valor booleano en la celda. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_3)(DateTime) | Coloca un valor DateTime en la celda. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_1)(double) | Coloca un valor double en la celda. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_2)(int) | Inserta un valor int en la celda. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_4)(object) | Inserta un valor de objeto en la celda. lo mismo que setValue(Object param_object) |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_5)(string) | Inserta un valor String en la celda. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_6)(string, bool) | Coloca un valor de cadena en la celda y convierte el valor a otro tipo de datos si es apropiado. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_7)(string, bool, bool) | Coloca un valor en la celda; si es apropiado, el valor se convertirá a otro tipo de datos y el formato numérico de la celda se restablecerá. |
| [PutValueAndSetFormatByValue](../../aspose.cells.griddesktop.data/gridcell/putvalueandsetformatbyvalue/)(string) | Establece el valor de la celda con un valor de cadena y establece el formato de la celda según este valor. |
| [SetCellValue](../../aspose.cells.griddesktop.data/gridcell/setcellvalue/)(object) | Si el valor es una fórmula, este método establece el valor de la celda como FormulaType, |
| [SetCustom](../../aspose.cells.griddesktop.data/gridcell/setcustom/)(string) | establece el formato personalizado, null o cadena vacía significa sin formato personalizado. |
| [SetFont](../../aspose.cells.griddesktop.data/gridcell/setfont/)(Font) | Establece la fuente en la celda. Para mejorar el rendimiento, implemente el método "SetFont", no implemente la propiedad "Font". |
| [SetFontColor](../../aspose.cells.griddesktop.data/gridcell/setfontcolor/)(Color) | Establece el color de fuente en la celda. Para mejorar el rendimiento, implemente el método "SetFontColor", no implemente la propiedad "FontColor". |
| [SetFormula](../../aspose.cells.griddesktop.data/gridcell/setformula/)(string, object) | Establezca la fórmula y el valor de la fórmula. |
| [SetNumberType](../../aspose.cells.griddesktop.data/gridcell/setnumbertype/)(int) | establezca el formato de visualización de números y fechas |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcell/setstyle/)(Style) | Establece el estilo en la celda. Para mejorar el rendimiento, implemente el método "SetStyle", no implemente la propiedad "Style". |
| override [ToString](../../aspose.cells.griddesktop.data/gridcell/tostring/)() | Devuelve una cadena que representa el objeto Cell actual. |
| [operator ==](../../aspose.cells.griddesktop.data/gridcell/op_equality/) |  |
| [operator !=](../../aspose.cells.griddesktop.data/gridcell/op_inequality/) |  |

### Ver también

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


