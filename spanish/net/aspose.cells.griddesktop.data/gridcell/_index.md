---
title: GridCell
second_title: Referencia de API de Aspose.Cells para .NET
description: Representa un objeto de celda.
type: docs
weight: 370
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
| [BoolValue](../../aspose.cells.griddesktop.data/gridcell/boolvalue) { get; } | Obtiene el valor booleano contenido en la celda. |
| [Column](../../aspose.cells.griddesktop.data/gridcell/column) { get; } | Obtiene el número de columna (basado en cero) de la celda. |
| [DateValue](../../aspose.cells.griddesktop.data/gridcell/datevalue) { get; } | Obtiene el valor DateTime contenido en la celda. |
| [DisplayStringValue](../../aspose.cells.griddesktop.data/gridcell/displaystringvalue) { get; } | Obtiene el valor de cadena con formato de esta celda. |
| [DoubleValue](../../aspose.cells.griddesktop.data/gridcell/doublevalue) { get; } | Obtiene el valor doble contenido en la celda. |
| [FloatValue](../../aspose.cells.griddesktop.data/gridcell/floatvalue) { get; } | Obtiene el valor flotante contenido en la celda. |
| [Formula](../../aspose.cells.griddesktop.data/gridcell/formula) { get; set; } | Obtiene o establece una fórmula delCell . |
| [HtmlString](../../aspose.cells.griddesktop.data/gridcell/htmlstring) { get; set; } | Obtiene y establece la cadena html que contiene datos y algunos formatos en esta celda. |
| [IntValue](../../aspose.cells.griddesktop.data/gridcell/intvalue) { get; } | Obtiene el valor entero contenido en la celda. |
| [IsStyleSet](../../aspose.cells.griddesktop.data/gridcell/isstyleset) { get; } | Indica si el estilo de la celda está configurado. Si devuelve falso, significa que esta celda tiene un formato de celda predeterminado. |
| [Location](../../aspose.cells.griddesktop.data/gridcell/location) { get; } |  |
| [Name](../../aspose.cells.griddesktop.data/gridcell/name) { get; } | Obtiene el nombre de la celda. Por ejemplo: A1, F102. |
| [Protected](../../aspose.cells.griddesktop.data/gridcell/protected) { get; set; } | Indica si la celda está protegida. Si el valor es "verdadero", el usuario no puede modificar la celda a través de la interfaz de usuario. Este atributo no tiene nada que ver con la propiedad Style.CellLocked y no se guardará en el archivo cuando datos de cuadrícula exportados. El valor predeterminado es "falso". |
| [Row](../../aspose.cells.griddesktop.data/gridcell/row) { get; } | Obtiene el número de fila (basado en cero) de la celda. |
| [StringValue](../../aspose.cells.griddesktop.data/gridcell/stringvalue) { get; } | Obtiene el valor de cadena contenido en la celda. |
| [Style](../../aspose.cells.griddesktop.data/gridcell/style) { get; set; } | Obtiene la copia del estilo de celda. establecer el estilo de la celda. |
| [Type](../../aspose.cells.griddesktop.data/gridcell/type) { get; } | devuelve el tipo de valor de celda, el significado puede ver GridCellValueType.java |
| [Value](../../aspose.cells.griddesktop.data/gridcell/value) { get; set; } | Obtiene el valor contenido en esta celda. |
| [Worksheet](../../aspose.cells.griddesktop.data/gridcell/worksheet) { get; } | Obtiene el objeto de la hoja de trabajo. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [ContainsExternalLink](../../aspose.cells.griddesktop.data/gridcell/containsexternallink)() | Indica si esta celda contiene un enlace externo. Solo se aplica cuando la celda es una celda de fórmula. |
| [Copy](../../aspose.cells.griddesktop.data/gridcell/copy)(GridCell) | Copia datos de una celda de origen. |
| [CopyStyle](../../aspose.cells.griddesktop.data/gridcell/copystyle)(Style) | copia el estilo y establece el estilo para la celda |
| override [Equals](../../aspose.cells.griddesktop.data/gridcell/equals)(object) |  |
| [GetCellArea](../../aspose.cells.griddesktop.data/gridcell/getcellarea)() |  |
| [GetFont](../../aspose.cells.griddesktop.data/gridcell/getfont)() | Obtiene la fuente de la celda. Cuando cambie la fuente, debe invocar el método "SetFont", para establecer la fuente en la celda. |
| [GetFontColor](../../aspose.cells.griddesktop.data/gridcell/getfontcolor)() | Obtiene el color de fuente de la celda. Cuando cambia el color, debe invocar el método "SetFontColor", para establecer el color de fuente en la celda. |
| override [GetHashCode](../../aspose.cells.griddesktop.data/gridcell/gethashcode)() |  |
| [GetStyle](../../aspose.cells.griddesktop.data/gridcell/getstyle)() | Obtiene el estilo de celda. Cuando cambie el estilo, debe invocar el método "SetStyle", para establecer el estilo en la celda. |
| [GetValidation](../../aspose.cells.griddesktop.data/gridcell/getvalidation)() | Obtiene la validación que se aplicó a esta celda. Si no se establece, devuelve nulo. |
| [GetWidthOfValue](../../aspose.cells.griddesktop.data/gridcell/getwidthofvalue)() | Obtiene el ancho del valor en unidades de píxeles. |
| [GetWorksheet](../../aspose.cells.griddesktop.data/gridcell/getworksheet)() | Obtiene la hoja de cálculo principal. |
| [IsErrorValue](../../aspose.cells.griddesktop.data/gridcell/iserrorvalue)() | Comprueba si una fórmula puede evaluar correctamente un resultado. |
| [IsFormula](../../aspose.cells.griddesktop.data/gridcell/isformula)() | Representa si la celda especificada contiene fórmula. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue)(bool) | Pone un valor booleano en la celda. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_3)(DateTime) | Pone un valor DateTime en la celda. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_1)(double) | Pone un valor doble en la celda. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_2)(int) | Pone un valor int en la celda. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_4)(object) | Pone un valor de objeto en la celda. Igual que setValue(Object param_object) |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_5)(string) | Pone un valor de cadena en la celda. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_6)(string, bool) | Pone un valor de cadena en la celda y convierte el valor a otro tipo de datos si corresponde. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_7)(string, bool, bool) | Pone un valor en la celda, si corresponde, el valor se convertirá a otro tipo de datos y se restablecerá el formato de número de la celda. |
| [PutValueAndSetFormatByValue](../../aspose.cells.griddesktop.data/gridcell/putvalueandsetformatbyvalue)(string) | Establece el valor de la celda con un valor de cadena y establece el formato de celda por este valor. |
| [SetCellValue](../../aspose.cells.griddesktop.data/gridcell/setcellvalue)(object) | Si el valor es una fórmula, este método establece el valor de la celda como FormulaType, |
| [SetCustom](../../aspose.cells.griddesktop.data/gridcell/setcustom)(string) | establece el formato personalizado, cadena nula o vacía significa que no hay formato personalizado. |
| [SetFont](../../aspose.cells.griddesktop.data/gridcell/setfont)(Font) | Establece la fuente en la celda. Para mejorar el rendimiento, implemente el método "SetFont", no implemente la propiedad "Fuente". |
| [SetFontColor](../../aspose.cells.griddesktop.data/gridcell/setfontcolor)(Color) | Establece el color de la fuente en la celda. Para mejorar el rendimiento, implemente el método "SetFontColor", no implemente la propiedad "FontColor". |
| [SetFormula](../../aspose.cells.griddesktop.data/gridcell/setformula)(string, object) | Establecer la fórmula y el valor de la fórmula. |
| [SetNumberType](../../aspose.cells.griddesktop.data/gridcell/setnumbertype)(int) | establecer el formato de visualización de números y fechas |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcell/setstyle)(Style) | Establece el estilo en la celda. Para mejorar el rendimiento, implemente el método "SetStyle", no implemente la propiedad "Estilo". |
| [ToString](../../aspose.cells.griddesktop.data/gridcell/tostring#tostring)() | Devuelve una cadena que representa el objeto Cell actual. |
| [operator ==](../../aspose.cells.griddesktop.data/gridcell/op_equality) |  |
| [operator !=](../../aspose.cells.griddesktop.data/gridcell/op_inequality) |  |

### Ver también

* espacio de nombres [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data)
* asamblea [Aspose.Cells.GridDesktop](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
