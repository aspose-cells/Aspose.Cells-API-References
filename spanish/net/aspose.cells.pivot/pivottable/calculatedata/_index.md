---
title: CalculateData
second_title: Referencia de API de Aspose.Cells para .NET
description: Calcula los datos de la tabla dinámica en celdas.
type: docs
weight: 760
url: /es/net/aspose.cells.pivot/pivottable/calculatedata/
---
## PivotTable.CalculateData method

Calcula los datos de la tabla dinámica en celdas.

```csharp
public void CalculateData()
```

### Observaciones

Cell.Value en el rango dinámico no podría devolver el resultado correcto si no se llama al método. Este método calcula los datos con un caché dinámico interno, no con la fuente de datos original. Por lo tanto, si se cambia la fuente de datos, llame a RefreshData () método primero.

### Ver también

* class [PivotTable](../../pivottable)
* espacio de nombres [Aspose.Cells.Pivot](../../pivottable)
* asamblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->