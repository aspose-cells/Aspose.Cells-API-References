---
title: GridCell
second_title: Referencia de API de Aspose.Cells para .NET
description: Representa un objeto de celda.
type: docs
weight: 150
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
| [BoolValue](../../aspose.cells.gridweb.data/gridcell/boolvalue) { get; } | Obtiene el valor booleano contenido en la celda. |
| [Column](../../aspose.cells.gridweb.data/gridcell/column) { get; } | Obtiene el número de columna (basado en cero) de la celda. |
| [DateValue](../../aspose.cells.gridweb.data/gridcell/datevalue) { get; } | Obtiene el valor DateTime contenido en la celda. |
| [DisplayStringValue](../../aspose.cells.gridweb.data/gridcell/displaystringvalue) { get; } | Obtiene el valor de cadena con formato de esta celda. |
| [DoubleValue](../../aspose.cells.gridweb.data/gridcell/doublevalue) { get; } | Obtiene el valor doble contenido en la celda. |
| [FloatValue](../../aspose.cells.gridweb.data/gridcell/floatvalue) { get; } | Obtiene el valor flotante contenido en la celda. |
| [Formula](../../aspose.cells.gridweb.data/gridcell/formula) { get; set; } | Obtiene o establece una fórmula delCell . |
| [HtmlString](../../aspose.cells.gridweb.data/gridcell/htmlstring) { get; set; } | Obtiene y establece la cadena html que contiene datos y algunos formatos en esta celda. |
| [IntValue](../../aspose.cells.gridweb.data/gridcell/intvalue) { get; } | Obtiene el valor entero contenido en la celda. |
| [IsStyleSet](../../aspose.cells.gridweb.data/gridcell/isstyleset) { get; } | Indica si el estilo de la celda está configurado. Si devuelve falso, significa que esta celda tiene un formato de celda predeterminado. |
| [Name](../../aspose.cells.gridweb.data/gridcell/name) { get; } | Obtiene el nombre de la celda. Por ejemplo: A1, F102. |
| [Row](../../aspose.cells.gridweb.data/gridcell/row) { get; } | Obtiene el número de fila (basado en cero) de la celda. |
| [StringValue](../../aspose.cells.gridweb.data/gridcell/stringvalue) { get; } | Obtiene el valor de cadena contenido en la celda. |
| [Style](../../aspose.cells.gridweb.data/gridcell/style) { get; set; } | Obtiene la copia del estilo de celda. establecer el estilo de la celda. |
| [Type](../../aspose.cells.gridweb.data/gridcell/type) { get; } | devuelve el tipo de valor de celda, el significado puede ver GridCellValueType.java |
| [Value](../../aspose.cells.gridweb.data/gridcell/value) { get; set; } | Obtiene el valor contenido en esta celda. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [ContainsExternalLink](../../aspose.cells.gridweb.data/gridcell/containsexternallink)() | Indica si esta celda contiene un enlace externo. Solo se aplica cuando la celda es una celda de fórmula. |
| [Copy](../../aspose.cells.gridweb.data/gridcell/copy)(GridCell) | Copia datos de una celda de origen. |
| [CopyStyle](../../aspose.cells.gridweb.data/gridcell/copystyle)(GridTableItemStyle) | copia el estilo y establece el estilo para la celda |
| [CreateComment](../../aspose.cells.gridweb.data/gridcell/createcomment)(string, string, bool) | Crea un objeto de comentario para una celda. |
| [CreateValidation](../../aspose.cells.gridweb.data/gridcell/createvalidation)(GridValidationType, bool) | Crea un objeto de validación para una celda. |
| override [Equals](../../aspose.cells.gridweb.data/gridcell/equals)(object) |  |
| [GetCellArea](../../aspose.cells.gridweb.data/gridcell/getcellarea)() |  |
| [GetComment](../../aspose.cells.gridweb.data/gridcell/getcomment)() | Obtener objeto de comentario en esta celda |
| override [GetHashCode](../../aspose.cells.gridweb.data/gridcell/gethashcode)() |  |
| [GetWidthOfValue](../../aspose.cells.gridweb.data/gridcell/getwidthofvalue)() | Obtiene el ancho del valor en unidades de píxeles. |
| [IsErrorValue](../../aspose.cells.gridweb.data/gridcell/iserrorvalue)() | Comprueba si una fórmula puede evaluar correctamente un resultado. |
| [IsFormula](../../aspose.cells.gridweb.data/gridcell/isformula)() | Representa si la celda especificada contiene fórmula. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue)(bool) | Pone un valor booleano en la celda. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_3)(DateTime) | Pone un valor DateTime en la celda. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_1)(double) | Pone un valor doble en la celda. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_2)(int) | Pone un valor int en la celda. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_4)(object) | Pone un valor de objeto en la celda. Igual que setValue(Object param_object) |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_5)(string) | Pone un valor de cadena en la celda. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_6)(string, bool) | Pone un valor de cadena en la celda y convierte el valor a otro tipo de datos si corresponde. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_7)(string, bool, bool) | Pone un valor en la celda, si corresponde, el valor se convertirá a otro tipo de datos y se restablecerá el formato de número de la celda. |
| [PutValueAndSetFormatByValue](../../aspose.cells.gridweb.data/gridcell/putvalueandsetformatbyvalue)(string) | Establece el valor de la celda con un valor de cadena y establece el formato de celda por este valor. |
| [RemoveComment](../../aspose.cells.gridweb.data/gridcell/removecomment)() | Elimina el objeto comentario de la celda. |
| [RemoveValidation](../../aspose.cells.gridweb.data/gridcell/removevalidation)() | Elimina el objeto de validación de la celda. |
| [SetBorder](../../aspose.cells.gridweb.data/gridcell/setborder)(WebBorderStyle) | Establece los bordes (superior, inferior, izquierdo y derecho) de una celda, todos los bordes tienen el mismo estilo de borde. |
| [SetCustom](../../aspose.cells.gridweb.data/gridcell/setcustom)(string) | establece el formato personalizado, cadena nula o vacía significa que no hay formato personalizado. |
| [SetFormula](../../aspose.cells.gridweb.data/gridcell/setformula)(string, object) | Establecer la fórmula y el valor de la fórmula. |
| [SetNumberType](../../aspose.cells.gridweb.data/gridcell/setnumbertype)(int) | establecer el formato de visualización de números y fechas |
| [ToString](../../aspose.cells.gridweb.data/gridcell/tostring#tostring)() | Devuelve una cadena que representa el objeto Cell actual. |
| [operator ==](../../aspose.cells.gridweb.data/gridcell/op_equality) |  |
| [operator !=](../../aspose.cells.gridweb.data/gridcell/op_inequality) |  |

### Ver también

* espacio de nombres [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data)
* asamblea [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
