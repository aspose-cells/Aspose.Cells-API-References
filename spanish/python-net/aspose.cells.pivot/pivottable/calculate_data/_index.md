---
title: calculate_data método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 40
url: /es/python-net/aspose.cells.pivot/pivottable/calculate_data/
is_root: false
---
##  calculate_data() {#}
Calcula los datos de la tabla dinámica a las celdas.



```python
def calculate_data(self):
    ...
```


###  Observaciones

Cell. El valor en el rango dinámico no podría devolver el resultado correcto si no se llama al método.
Este método calcula los datos con un caché dinámico interno, no con una fuente de datos original.
Entonces, si se cambia la fuente de datos, llame primero al método RefreshData().


###  Ver también
* módulo [aspose.cells.pivot](../../)
* clase [PivotTable](/cells/es/python-net/aspose.cells.pivot/pivottable)
