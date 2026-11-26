---
title: "Clase GridCell"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.GridWeb.Data.GridCell. Representa un objeto celda."
type: docs
url: /es/net/aspose.cells.gridweb.data/gridcell/
---
## GridCell class

Representa un objeto de celda.

```csharp
public class GridCell
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BoolValue](../../aspose.cells.gridweb.data/gridcell/boolvalue/) { get; } | Obtiene el valor booleano contenido en la celda. |
| [Column](../../aspose.cells.gridweb.data/gridcell/column/) { get; } | Obtiene el número de columna (basado en cero) de la celda. |
| [DateValue](../../aspose.cells.gridweb.data/gridcell/datevalue/) { get; } | Obtiene el valor DateTime contenido en la celda. |
| [DisplayStringValue](../../aspose.cells.gridweb.data/gridcell/displaystringvalue/) { get; } | Obtiene el valor de cadena formateado de esta celda. |
| [DoubleValue](../../aspose.cells.gridweb.data/gridcell/doublevalue/) { get; } | Obtiene el valor double contenido en la celda. |
| [FloatValue](../../aspose.cells.gridweb.data/gridcell/floatvalue/) { get; } | Obtiene el valor float contenido en la celda. |
| [Formula](../../aspose.cells.gridweb.data/gridcell/formula/) { get; set; } | Obtiene o establece una fórmula del `GridCell`. |
| [HtmlString](../../aspose.cells.gridweb.data/gridcell/htmlstring/) { get; set; } | Obtiene y establece la cadena html que contiene datos y algunos formatos en esta celda. |
| [IntValue](../../aspose.cells.gridweb.data/gridcell/intvalue/) { get; } | Obtiene el valor entero contenido en la celda. |
| [IsStyleSet](../../aspose.cells.gridweb.data/gridcell/isstyleset/) { get; } | Indica si el estilo de la celda está establecido. Si devuelve false, significa que esta celda tiene un formato de celda predeterminado. |
| [Name](../../aspose.cells.gridweb.data/gridcell/name/) { get; } | Obtiene el nombre de la celda. Por ejemplo: A1, F102. |
| [Row](../../aspose.cells.gridweb.data/gridcell/row/) { get; } | Obtiene el número de fila (basado en cero) de la celda. |
| [StringValue](../../aspose.cells.gridweb.data/gridcell/stringvalue/) { get; } | Obtiene el valor de cadena contenido en la celda. |
| [Style](../../aspose.cells.gridweb.data/gridcell/style/) { get; set; } | Obtiene la copia del estilo de la celda. establece el estilo para la celda. |
| [Type](../../aspose.cells.gridweb.data/gridcell/type/) { get; } | devuelve el tipo de valor de la celda, el significado se puede ver en GridCellValueType.java |
| [Value](../../aspose.cells.gridweb.data/gridcell/value/) { get; set; } | Obtiene el valor contenido en esta celda. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [ContainsExternalLink](../../aspose.cells.gridweb.data/gridcell/containsexternallink/)() | Indica si esta celda contiene un enlace externo. Solo se aplica cuando la celda es una celda de fórmula. |
| [Copy](../../aspose.cells.gridweb.data/gridcell/copy/)(GridCell) | Copia datos de una celda origen. |
| [CopyStyle](../../aspose.cells.gridweb.data/gridcell/copystyle/)(GridTableItemStyle) | copia el estilo y establece el estilo para la celda |
| [CreateComment](../../aspose.cells.gridweb.data/gridcell/createcomment/)(string, string, bool) | Crea un objeto de comentario para una celda. |
| [CreateValidation](../../aspose.cells.gridweb.data/gridcell/createvalidation/)(GridValidationType, bool) | Crea un objeto de validación para una celda. |
| override [Equals](../../aspose.cells.gridweb.data/gridcell/equals/)(object) | Comprueba si este objeto se refiere a la misma celda que otro objeto de celda. |
| [GetComment](../../aspose.cells.gridweb.data/gridcell/getcomment/)() | Obtener objeto de comentario en esta celda |
| override [GetHashCode](../../aspose.cells.gridweb.data/gridcell/gethashcode/)() | Sirve como función hash para un tipo particular. |
| [GetWidthOfValue](../../aspose.cells.gridweb.data/gridcell/getwidthofvalue/)() | Obtiene el ancho del valor en unidades de píxeles. |
| [IsErrorValue](../../aspose.cells.gridweb.data/gridcell/iserrorvalue/)() | Comprueba si una fórmula puede evaluar correctamente un resultado. |
| [IsFormula](../../aspose.cells.gridweb.data/gridcell/isformula/)() | Representa si la celda especificada contiene una fórmula. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue)(bool) | Coloca un valor booleano en la celda. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_3)(DateTime) | Coloca un valor DateTime en la celda. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_1)(double) | Coloca un valor double en la celda. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_2)(int) | Inserta un valor int en la celda. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_4)(object) | Inserta un valor de objeto en la celda. lo mismo que setValue(Object param_object) |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_5)(string) | Inserta un valor String en la celda. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_6)(string, bool) | Coloca un valor de cadena en la celda y convierte el valor a otro tipo de datos si es apropiado. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_7)(string, bool, bool) | Coloca un valor en la celda; si es apropiado, el valor se convertirá a otro tipo de datos y el formato numérico de la celda se restablecerá. |
| [PutValueAndSetFormatByValue](../../aspose.cells.gridweb.data/gridcell/putvalueandsetformatbyvalue/)(string) | Establece el valor de la celda con un valor de cadena y establece el formato de la celda según este valor. |
| [RemoveComment](../../aspose.cells.gridweb.data/gridcell/removecomment/)() | Elimina el objeto de comentario de la celda. |
| [RemoveValidation](../../aspose.cells.gridweb.data/gridcell/removevalidation/)() | Elimina el objeto de validación de la celda. |
| [SetBorder](../../aspose.cells.gridweb.data/gridcell/setborder/)(WebBorderStyle) | Establece bordes (superior, inferior, izquierdo y derecho) para una celda; todos los bordes tienen el mismo estilo de borde. |
| [SetCustom](../../aspose.cells.gridweb.data/gridcell/setcustom/)(string) | establece el formato personalizado, null o cadena vacía significa sin formato personalizado. |
| [SetFormula](../../aspose.cells.gridweb.data/gridcell/setformula/)(string, object) | Establezca la fórmula y el valor de la fórmula. |
| [SetNumberType](../../aspose.cells.gridweb.data/gridcell/setnumbertype/)(int) | establezca el formato de visualización de números y fechas |
| [ToString](../../aspose.cells.gridweb.data/gridcell/tostring/#tostring)() | Devuelve una cadena que representa el objeto Cell actual. |
| [operator ==](../../aspose.cells.gridweb.data/gridcell/op_equality/) |  |
| [operator !=](../../aspose.cells.gridweb.data/gridcell/op_inequality/) |  |

### Ver también

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


