---
title: CalculatedValue
second_title: Referencia de API de Aspose.Cells para .NET
description: Obtiene o establece el valor calculado para esta función.
type: docs
weight: 10
url: /es/net/aspose.cells/calculationdata/calculatedvalue/
---
## CalculationData.CalculatedValue property

Obtiene o establece el valor calculado para esta función.

```csharp
public object CalculatedValue { get; set; }
```

### Observaciones

El usuario debe establecer esta propiedad en su motor de cálculo personalizado para aquellas funciones que admite el motor, y el valor establecido se devolverá cuando obtenga esta propiedad más adelante. El valor establecido puede ser cualquier valor de esos objetos que se pueden establecer en una celda ( Cell.Value). Y también puede ser una matriz de este tipo de valores, o un Rango, Nombre, ReferredArea. Obtener esta propiedad antes de la configuración hará que la función sea calculada por el motor de cálculo predeterminado de Aspose.Cells y el calculado se devolverá el valor.

### Ver también

* class [CalculationData](../../calculationdata)
* espacio de nombres [Aspose.Cells](../../calculationdata)
* asamblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
