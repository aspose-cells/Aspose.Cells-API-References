---
title: "GridDesktop.AlwasysRecalculateAllFormulas"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de GridDesktop. Obtiene o establece un valor que indica si necesitamos ejecutar todas las fórmulas cuando actualizamos el valor de una celda y este afecta a otras, y esas a su vez afectan a más, lo que obliga a recalcular todas las celdas, similar al efecto mariposa; requiere muchas operaciones de pila y produce un rendimiento muy bajo, como en CELLSNET41921. Este problema contiene el archivo que muestra este escenario; sería mejor ejecutar todas las fórmulas, ya que al hacerlo podemos aplicar alguna optimización"
type: docs
url: /es/net/aspose.cells.griddesktop/griddesktop/alwasysrecalculateallformulas/
---
## GridDesktop.AlwasysRecalculateAllFormulas property

Obtiene o establece un valor que indica si necesitamos ejecutar todas las fórmulas, ya que al ejecutar todas las fórmulas, al actualizar el valor de una celda, afecta a otras, y esas a otras, y así sucesivamente, lo que hace que todas las celdas necesiten recalcularse, como el efecto mariposa, requiere muchas operaciones de pila, lo que produce un rendimiento muy bajo, como en CELLSNET-41921; este problema contiene el archivo que muestra este escenario. Es mejor ejecutar todas las fórmulas, ya que al hacerlo podemos aplicar algunas optimizaciones.

```csharp
public bool AlwasysRecalculateAllFormulas { get; set; }
```

### Ver también

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


