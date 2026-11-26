---
title: "Clase Validation"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.GridWeb.Validation."
type: docs
url: /es/net/aspose.cells.gridweb/validation/
---
## Validation class

```csharp
[Obsolete("This class is obsolete; use  GridValidation instead")]
public class Validation : CellAttachObject
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [Validation](validation/#constructor)() | El constructor predeterminado. |
| [Validation](validation/#constructor_1)(GridValidation) |  |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Cell](../../aspose.cells.gridweb.data/cellattachobject/cell/) { get; } | Obtiene la celda relativa del objeto. (Heredado de [`CellAttachObject`](../../aspose.cells.gridweb.data/cellattachobject/).) |
| [ClientValidationFunction](../../aspose.cells.gridweb/validation/clientvalidationfunction/) { get; set; } | Obtiene o establece el nombre de la función JavaScript de validación del cliente. |
| [ClientValidationOpType](../../aspose.cells.gridweb/validation/clientvalidationoptype/) { get; set; } | Obtiene o establece el tipo de operación de validación, Between/NotBetween/Equal/NotEqual/Greater/GreaterOrEqual/Less/LessOrEqual. |
| [ClientValidationValue1](../../aspose.cells.gridweb/validation/clientvalidationvalue1/) { get; set; } | Obtiene o establece el valor objetivo del operador 1 |
| [ClientValidationValue2](../../aspose.cells.gridweb/validation/clientvalidationvalue2/) { get; set; } | Obtiene o establece el valor objetivo del operador 2 |
| [IsRequired](../../aspose.cells.gridweb/validation/isrequired/) { get; set; } | Obtiene o establece si el valor de la celda es obligatorio. |
| [RegEx](../../aspose.cells.gridweb/validation/regex/) { get; set; } | Obtiene o establece la cadena de expresión regular. |
| [ValueArray](../../aspose.cells.gridweb/validation/valuearray/) { get; set; } |  |
| [ValueList](../../aspose.cells.gridweb/validation/valuelist/) { get; } | Obtiene el objeto de lista de valores. |
| [ValueText](../../aspose.cells.gridweb/validation/valuetext/) { get; set; } | Solo se usa en tiempo de diseño. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [LoadValueList](../../aspose.cells.gridweb/validation/loadvaluelist/)(DataView, string, string, bool) | Carga la lista de valores desde un objeto DataView. Puede especificar el campo de valor y el campo de texto del DataView. Cada par de valor y texto se combinará en una cadena, con una coma entre ellos. |

### Observaciones

NOTA: Esta clase está ahora obsoleta. Por favor use GridValidation en su lugar. Esta clase será eliminada después de 6 meses desde agosto de 2014. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

### Ver también

* class [CellAttachObject](../../aspose.cells.gridweb.data/cellattachobject/)
* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


