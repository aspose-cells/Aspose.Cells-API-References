---
title: CalculationId
second_title: Referencia de API de Aspose.Cells para .NET
description: Especifica la versión del motor de cálculo utilizado para calcular valores en el libro.
type: docs
weight: 30
url: /es/net/aspose.cells/formulasettings/calculationid/
---
## FormulaSettings.CalculationId property

Especifica la versión del motor de cálculo utilizado para calcular valores en el libro.

```csharp
public string CalculationId { get; set; }
```

### Observaciones

Esta propiedad es solo para guardar la configuración en el archivo de hoja de cálculo resultante para que otras aplicaciones (como ms excel) puedan actuar en consecuencia al cargar y manipular el archivo resultante. En el caso de ms excel, si el valor de esta propiedad es menor que el identificador del motor de recálculo asociado con la aplicación que abre el archivo resultante, la aplicación volverá a calcular los resultados de todas las fórmulas en este libro de trabajo inmediatamente después de cargar el archivo. Por consideraciones de rendimiento para la mayoría de las aplicaciones de los usuarios, no calculamos ninguna fórmula en el libro de trabajo automáticamente, sin importar qué valor se haya establecido para esta propiedad.

### Ver también

* class [FormulaSettings](../../formulasettings)
* espacio de nombres [Aspose.Cells](../../formulasettings)
* asamblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
