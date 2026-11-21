---
title: "LightCellsDataProvider"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa el proveedor de datos para guardar archivos de hoja de cálculo grandes en modo ligero."
type: docs
url: /es/java/com.aspose.cells/lightcellsdataprovider/
---
```
public interface LightCellsDataProvider
```

Representa el proveedor de datos para guardar archivos de hoja de cálculo grandes en modo ligero.

**Remarks**

Al guardar un libro de trabajo en este modo, se comprobará [startSheet(int)](../../com.aspose.cells/lightcellsdataprovider\#startSheet-int-) al guardar cada hoja de cálculo en el libro. Para una hoja, si [startSheet(int)](../../com.aspose.cells/lightcellsdataprovider\#startSheet-int-) devuelve true, entonces todos los datos y propiedades que se deben guardar para las filas/celdas de esta hoja serán proporcionados por la implementación de esta interfaz. En primer lugar, se llamará a [nextRow()](../../com.aspose.cells/lightcellsdataprovider\#nextRow--) para obtener el índice de la siguiente fila a guardar. Si se devuelve un índice de fila válido (el índice de fila debe estar en orden ascendente para las filas que se van a guardar), entonces un objeto Row que representa esa fila será proporcionado por [startRow(Row)](../../com.aspose.cells/lightcellsdataprovider\#startRow-Row-) para que la implementación establezca sus propiedades. Para una fila, se comprobará primero [nextCell()](../../com.aspose.cells/lightcellsdataprovider\#nextCell--). Si se devuelve un índice de columna válido (el índice de columna debe estar en orden ascendente para todas las celdas de la fila actual), entonces un objeto Cell que representa esa celda será proporcionado por [startCell(Cell)](../../com.aspose.cells/lightcellsdataprovider\#startCell-Cell-) para que la implementación establezca sus datos y propiedades. Después de [startCell(Cell)](../../com.aspose.cells/lightcellsdataprovider\#startCell-Cell-) la celda se guardará directamente en el archivo de hoja de cálculo resultante. Luego se comprobará y procesará la siguiente celda.

Tenga en cuenta que el usuario solo debe actualizar valores y propiedades del objeto Row/Cell actual proporcionado por el método correspondiente. Debido a que los datos de las celdas se escriben en el archivo resultante de forma secuencial, la mayoría de los demás objetos pueden haber sido escritos en el archivo resultante, o haberse recopilado y escrito algunos datos globales para ellos. Por lo tanto, cuando el usuario actualiza otros objetos mientras se guardan los datos de las celdas, esas operaciones pueden no afectar los datos guardados. O peor aún, esas operaciones pueden causar que datos inconsistentes se guarden en el archivo resultante y finalmente corrompan el archivo. Así que, para todos los demás objetos como formas, ancho de columnas y estilos, formatos condicionales, ...etc., por favor no los manipule en ningún método de esta implementación. En su lugar, adminístrelos y ajústelos al estado final antes de llamar al método "Save" del Workbook.
## Métodos

| Método | Descripción |
| --- | --- |
| [isGatherString()](#isGatherString--) | Comprueba si el valor de cadena actual de la celda necesita recopilarse en un grupo global. |
| [nextCell()](#nextCell--) | Obtiene la siguiente celda que se guardará. |
| [nextRow()](#nextRow--) | Obtiene la siguiente fila que se guardará. |
| [startCell(Cell cell)](#startCell-com.aspose.cells.Cell-) | Comienza a guardar los datos de una celda. |
| [startRow(Row row)](#startRow-com.aspose.cells.Row-) | Comienza a guardar los datos de una fila. |
| [startSheet(int sheetIndex)](#startSheet-int-) | Comienza a guardar una hoja de cálculo. |
### isGatherString() {#isGatherString--}
```
public abstract boolean isGatherString()
```


Comprueba si el valor de cadena actual de la celda necesita recopilarse en un grupo global.

**Remarks**

Recopilar valores de cadena solo será ventajoso cuando haya muchos valores de cadena duplicados para las celdas proporcionadas por esta implementación. En esta situación, recopilar cadenas ahorrará mucha memoria y generará un archivo resultante más pequeño. Si hay muchos valores de cadena para las celdas proporcionadas por LightCellsDataProvider pero pocos son iguales, recopilar cadenas consumirá más memoria y tiempo y no tendrá ventaja para el archivo resultante.

**Returns:**
boolean - true si el valor de cadena necesita recopilarse en un grupo global para el archivo resultante.
### nextCell() {#nextCell--}
```
public abstract int nextCell()
```


Obtiene la siguiente celda que se guardará.

**Remarks**

Se llamará al principio de guardar una celda.

**Returns:**
int - índice de columna de la siguiente celda que se guardará. -1 indica que se ha alcanzado el final de los datos de la fila actual y no hay más celdas de la fila actual que guardar.
### nextRow() {#nextRow--}
```
public abstract int nextRow()
```


Obtiene la siguiente fila que se guardará.

**Remarks**

Se llamará al principio de guardar una fila y sus datos de celdas (antes de [startRow(Row)](../../com.aspose.cells/lightcellsdataprovider\#startRow-Row-)).

**Returns:**
int - el siguiente índice de fila que se guardará. -1 indica que se ha alcanzado el final de los datos de la hoja actual y no hay más filas de la hoja actual que guardar.
### startCell(Cell cell) {#startCell-com.aspose.cells.Cell-}
```
public abstract void startCell(Cell cell)
```


Comienza a guardar los datos de una celda.

**Remarks**

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | Objeto Cell para que la implementación rellene datos. Su índice de columna es el valor devuelto de la última llamada a [nextCell()](../../com.aspose.cells/lightcellsdataprovider\#nextCell--). Si la celda ha sido inicializada en el modelo interno de celdas, se utilizará el objeto Cell existente. De lo contrario, se usará un objeto Cell temporal para que la implementación rellene datos. |

### startRow(Row row) {#startRow-com.aspose.cells.Row-}
```
public abstract void startRow(Row row)
```


Comienza a guardar los datos de una fila.

**Remarks**

Se llamará al principio de guardar una fila y sus datos de celdas. Si la fila actual tiene algunas propiedades personalizadas como altura, estilo, ...etc., la implementación debe establecer esas propiedades en el objeto Row proporcionado aquí.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| row | [Row](../../com.aspose.cells/row) | Objeto Row para que la implementación rellene datos. Su índice de fila es el valor devuelto de la última llamada a [nextRow()](../../com.aspose.cells/lightcellsdataprovider\#nextRow--). Si la fila ha sido inicializada en el modelo interno de celdas, se utilizará el objeto Row existente. De lo contrario, se usará un objeto Row temporal para que la implementación rellene datos. |

### startSheet(int sheetIndex) {#startSheet-int-}
```
public abstract boolean startSheet(int sheetIndex)
```


Comienza a guardar una hoja de cálculo.

**Remarks**

Se llamará al principio de guardar una hoja de cálculo durante el guardado de un libro. Si el proveedor necesita referirse a *`sheetIndex`* más tarde en los métodos startRow(Row) o startCell(Cell), es decir, si el proceso necesita saber qué hoja de cálculo se está procesando, la implementación debe retener el valor de *`sheetIndex`* aquí.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetIndex | int | índice de la hoja actual que se guardará. |

**Returns:**
boolean - true si este proveedor proporcionará datos para la hoja dada; false si la hoja dada debe usar su modelo de datos normal (Cells).
