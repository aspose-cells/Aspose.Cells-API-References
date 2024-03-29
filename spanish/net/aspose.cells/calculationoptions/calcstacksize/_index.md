---
title: CalcStackSize
second_title: Referencia de API de Aspose.Cells para .NET
description: Especifica el tamaño de la pila para calcular celdas recursivamente.
type: docs
weight: 20
url: /es/net/aspose.cells/calculationoptions/calcstacksize/
---
## CalculationOptions.CalcStackSize property

Especifica el tamaño de la pila para calcular celdas recursivamente.

```csharp
public int CalcStackSize { get; set; }
```

### Observaciones

Cuando hay una gran cantidad de celdas que deben calcularse recursivamente en el árbol de dependencias, StackOverflowException se puede generar en el proceso de cálculo. Si es así, el usuario debe especificar un valor más pequeño para esta propiedad. Para tal situación, el usuario debe determinar el valor adecuado para esta propiedad de acuerdo con las fórmulas y los datos reales. Un valor demasiado pequeño puede causar una degradación del rendimiento para el cálculo de la fórmula.

### Ver también

* class [CalculationOptions](../../calculationoptions)
* espacio de nombres [Aspose.Cells](../../calculationoptions)
* asamblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
