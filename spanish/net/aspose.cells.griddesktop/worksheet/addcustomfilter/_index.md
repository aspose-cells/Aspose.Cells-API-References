---
title: "Worksheet.AddCustomFilter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Worksheet. Añade un filtro personalizado para el rango de filas especificado desde la fila inicial hasta la fila final"
type: docs
url: /es/net/aspose.cells.griddesktop/worksheet/addcustomfilter/
---
## AddCustomFilter(int, int, object[], GridFilterOperatorType[]) {#addcustomfilter}

Agrega un filtro personalizado para el rango de filas especificado desde la fila de inicio hasta la fila final.

```csharp
public void AddCustomFilter(int startrow, int startcolumn, object[] critiras, 
    GridFilterOperatorType[] filterOperatorTypes)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startrow | Int32 | El startrow del rango de filtro |
| startcolumn | Int32 | El startcolumn del rango de filtro |
| critiras | Object[] | La matriz de critira para las columnas, cada una se aplica a cada columna |
| filterOperatorTypes | GridFilterOperatorType[] | La matriz de tipos de operación de filtro para las columnas, cada una se aplica a cada columna |

### Ver también

* enum [GridFilterOperatorType](../../../aspose.cells.griddesktop.data/gridfilteroperatortype/)
* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## AddCustomFilter(int, string) {#addcustomfilter_1}

Agregar filtro personalizado para la fila especificada.

```csharp
public void AddCustomFilter(int row, string critira)
```

### Observaciones

La cadena de criterios de filtro. Observe que usamos , y ; como caracteres de separación, por lo que el valor de la celda no debe contener esos caracteres. A continuación se muestran ejemplos de la cadena de criterios: //column 0 with value 12.3 CELL0 = 12.3 //column 1 with value ABC CELL1 = ABC //column 0 with value 123 or 456 or ABC and column 1 with value ABC CELL0 = 123,456,ABC; CELL1 = ABC

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


