---
title: AddCustomFilter
second_title: Referencia de API de Aspose.Cells para .NET
description: Agregue un filtro personalizado para el rango de filas especificado desde la fila inicial hasta la fila final.
type: docs
weight: 450
url: /es/net/aspose.cells.griddesktop/worksheet/addcustomfilter/
---
## AddCustomFilter(int, int, object[], GridFilterOperatorType[]) {#addcustomfilter}

Agregue un filtro personalizado para el rango de filas especificado desde la fila inicial hasta la fila final.

```csharp
public void AddCustomFilter(int startrow, int startcolumn, object[] critiras, 
    GridFilterOperatorType[] filterOperatorTypes)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| startrow | Int32 | La fila de inicio de la gama de filtros |
| startcolumn | Int32 | La columna de inicio del rango de filtro. |
| critiras | Object[] | La matriz de criterios para las columnas, cada una se aplica a cada columna. |
| filterOperatorTypes | GridFilterOperatorType[] | La matriz de tipo de operación de filtro para las columnas, cada una se aplica a cada columna |

### Ver también

* enum [GridFilterOperatorType](../../../aspose.cells.griddesktop.data/gridfilteroperatortype)
* class [Worksheet](../../worksheet)
* espacio de nombres [Aspose.Cells.GridDesktop](../../worksheet)
* asamblea [Aspose.Cells.GridDesktop](../../../)

---

## AddCustomFilter(int, string) {#addcustomfilter_1}

Agregar filtro personalizado para la fila especificada.

```csharp
public void AddCustomFilter(int row, string critira)
```

### Observaciones

La cadena de criterios de filtro. aviso que usamos , y ; como carácter dividido, por lo que el valor de la celda no debe contener esos caracteres divididos a continuación se encuentran los ejemplos de cadenas de criterios: //columna 0 con valor 12.3 CELL0 = 12.3 //columna 1 con valor ABC CELL1 = ABC //columna 0 con valor 123 o 456 o ABC y columna 1 con valor ABC CELL0 = 123,456,ABC; CELDA1 = ABC

### Ver también

* class [Worksheet](../../worksheet)
* espacio de nombres [Aspose.Cells.GridDesktop](../../worksheet)
* asamblea [Aspose.Cells.GridDesktop](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
