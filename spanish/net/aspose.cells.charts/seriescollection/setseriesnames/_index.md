---
title: SetSeriesNames
second_title: Referencia de API de Aspose.Cells para .NET
description: Establece el nombre de todas las series del gráfico.
type: docs
weight: 110
url: /es/net/aspose.cells.charts/seriescollection/setseriesnames/
---
## SeriesCollection.SetSeriesNames method

Establece el nombre de todas las series del gráfico.

```csharp
public void SetSeriesNames(int startIndex, string area, bool isVertical)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| startIndex | Int32 | El índice de la primera serie a la que desea establecer el nombre. |
| area | String | Especifica el área para el nombre de la serie. |
| isVertical | Boolean | &gt;Especifica si trazar la serie a partir de un rango de valores de celda por fila o por columna. |

### Observaciones

Si el índice de inicio es mayor que el recuento de la serie, regresará y no hará nada.Si establece datos en celdas contiguas, use dos puntos para separarlas. Por ejemplo, $C$2:$C$5.Si establece datos en celdas contiguas, use una coma para separarlas. Por ejemplo, ($C$2,$D$5).

### Ver también

* class [SeriesCollection](../../seriescollection)
* espacio de nombres [Aspose.Cells.Charts](../../seriescollection)
* asamblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
