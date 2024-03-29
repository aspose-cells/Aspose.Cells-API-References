---
title: Merge
second_title: Referencia de API de Aspose.Cells para .NET
description: Combina un rango específico de celdas en una sola celda.
type: docs
weight: 1180
url: /es/net/aspose.cells/cells/merge/
---
## Merge(int, int, int, int) {#merge}

Combina un rango específico de celdas en una sola celda.

```csharp
public void Merge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| firstRow | Int32 | Primera fila de este rango (basado en cero) |
| firstColumn | Int32 | Primera columna de este rango (basado en cero) |
| totalRows | Int32 | Número de filas (basado en uno) |
| totalColumns | Int32 | Número de columnas (basado en uno) |

### Observaciones

Hace referencia a la celda combinada a través de la dirección de la celda superior izquierda en el rango.

### Ver también

* class [Cells](../../cells)
* espacio de nombres [Aspose.Cells](../../cells)
* asamblea [Aspose.Cells](../../../)

---

## Merge(int, int, int, int, bool) {#merge_1}

Combina un rango específico de celdas en una sola celda.

```csharp
public void Merge(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    bool mergeConflict)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| firstRow | Int32 | Primera fila de este rango (basado en cero) |
| firstColumn | Int32 | Primera columna de este rango (basado en cero) |
| totalRows | Int32 | Número de filas (basado en uno) |
| totalColumns | Int32 | Número de columnas (basado en uno) |
| mergeConflict | Boolean | Combinar rangos combinados en conflicto. |

### Observaciones

Hace referencia a la celda combinada a través de la dirección de la celda superior izquierda en el rango. Si mergeConflict es verdadero y el rango combinado entra en conflicto con otras celdas combinadas, se eliminarán automáticamente otras celdas combinadas.

### Ver también

* class [Cells](../../cells)
* espacio de nombres [Aspose.Cells](../../cells)
* asamblea [Aspose.Cells](../../../)

---

## Merge(int, int, int, int, bool, bool) {#merge_2}

Combina un rango específico de celdas en una sola celda.

```csharp
public void Merge(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    bool checkConflict, bool mergeConflict)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| firstRow | Int32 | Primera fila de este rango (basado en cero) |
| firstColumn | Int32 | Primera columna de este rango (basado en cero) |
| totalRows | Int32 | Número de filas (basado en uno) |
| totalColumns | Int32 | Número de columnas (basado en uno) |
| checkConflict | Boolean | Indica si la verificación de las celdas combinadas se cruza con otras celdas combinadas |
| mergeConflict | Boolean | Combinar rangos combinados en conflicto. |

### Observaciones

Hace referencia a la celda combinada a través de la dirección de la celda superior izquierda en el rango. Si mergeConflict es verdadero y el rango combinado entra en conflicto con otras celdas combinadas, se eliminarán automáticamente otras celdas combinadas.

### Ver también

* class [Cells](../../cells)
* espacio de nombres [Aspose.Cells](../../cells)
* asamblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
