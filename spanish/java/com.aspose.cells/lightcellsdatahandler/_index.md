---
title: "LightCellsDataHandler"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa el manejador de datos de celdas para leer archivos de hoja de cálculo grandes en modo ligero."
type: docs
url: /es/java/com.aspose.cells/lightcellsdatahandler/
---
```
public interface LightCellsDataHandler
```

Representa el manejador de datos de celdas para leer archivos de hoja de cálculo grandes en modo ligero.

**Remarks**

Al leer un libro de trabajo en este modo, se comprobará [startSheet(Worksheet)](../../com.aspose.cells/lightcellsdatahandler\#startSheet-Worksheet-) al leer cada hoja de cálculo del libro. Para una hoja, si [startSheet(Worksheet)](../../com.aspose.cells/lightcellsdatahandler\#startSheet-Worksheet-) devuelve true, entonces todos los datos y propiedades de filas/celdas de esa hoja serán verificados y procesados por la implementación de esta interfaz. Para cada fila, se llamará a [startRow(int)](../../com.aspose.cells/lightcellsdatahandler\#startRow-int-) para comprobar si necesita ser procesada. Si una fila necesita ser procesada, sus propiedades se leerán primero y el usuario podrá acceder a ellas mediante [processRow(Row)](../../com.aspose.cells/lightcellsdatahandler\#processRow-Row-). Si también es necesario procesar las celdas de la fila, entonces [processRow(Row)](../../com.aspose.cells/lightcellsdatahandler\#processRow-Row-) debe devolver true y luego se llamará a [startCell(int)](../../com.aspose.cells/lightcellsdatahandler\#startCell-int-) para cada celda existente en esa fila para comprobar si una celda necesita ser procesada. Si una celda necesita ser procesada, se llamará a [processCell(Cell)](../../com.aspose.cells/lightcellsdatahandler\#processCell-Cell-) para procesar la celda mediante la implementación de esta interfaz.

Por favor, tenga en cuenta que el usuario solo debe operar sobre los valores y propiedades del objeto Row/Cell actual proporcionado por el método correspondiente. Debido a que los datos de las celdas se leen del archivo de plantilla de forma secuencial, la mayoría de los demás objetos pueden ser restablecidos/actualizados más tarde después de que se hayan cargado los datos de las celdas. Por lo tanto, cuando el usuario opere con otros objetos en esta implementación, esas operaciones pueden no afectar a los objetos existentes en el libro de trabajo. O peor aún, esas operaciones pueden causar datos inconsistentes en el libro y provocar problemas o excepciones inesperadas más adelante. Así que, para todos los demás objetos como formas, ancho de columnas y estilos, formatos condicionales, ...etc., por favor no los manipule en ningún método de esta implementación. En su lugar, adminístrelos después de que el libro de trabajo haya sido construido.
## Métodos

| Método | Descripción |
| --- | --- |
| [processCell(Cell cell)](#processCell-com.aspose.cells.Cell-) | Comienza a procesar una celda. |
| [processRow(Row row)](#processRow-com.aspose.cells.Row-) | Comienza a procesar una fila. |
| [startCell(int columnIndex)](#startCell-int-) | Se prepara para procesar una celda. |
| [startRow(int rowIndex)](#startRow-int-) | Se prepara para procesar una fila. |
| [startSheet(Worksheet sheet)](#startSheet-com.aspose.cells.Worksheet-) | Comienza a procesar una hoja de cálculo. |
### processCell(Cell cell) {#processCell-com.aspose.cells.Cell-}
```
public abstract boolean processCell(Cell cell)
```


Comienza a procesar una celda.

**Remarks**

Se llamará después de que se hayan leído los datos de una celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | Objeto Cell que se está procesando actualmente |

**Returns:**
boolean - indica si esta celda necesita mantenerse en el modelo de celdas de la hoja actual. Normalmente debería ser false para que todas las celdas no se mantengan en memoria después de ser procesadas y así se ahorre memoria. Para algunos propósitos especiales, como cuando el usuario necesita acceder a ciertas celdas más tarde después de que todo el libro de trabajo haya sido procesado, el usuario puede hacer que este método devuelva true para conservar esas celdas especiales en el modelo Cells y acceder a ellas posteriormente mediante APIs como Cells[row, column]. Sin embargo, mantener los datos de las celdas en el modelo Cells requerirá más memoria y, si se conservan todas las celdas, la lectura del archivo de plantilla en modo LightCells será igual que leerlo de forma normal.
### processRow(Row row) {#processRow-com.aspose.cells.Row-}
```
public abstract boolean processRow(Row row)
```


Comienza a procesar una fila.

**Remarks**

Se llamará después de que se hayan leído las propiedades de la fila, como altura, estilo, ...etc. Sin embargo, las celdas de esta fila aún no se han leído.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| row | [Row](../../com.aspose.cells/row) | Objeto Row que se está procesando actualmente. |

**Returns:**
boolean - indica si las celdas de esta fila necesitan ser procesadas. false para ignorar todas las celdas de esta fila.
### startCell(int columnIndex) {#startCell-int-}
```
public abstract boolean startCell(int columnIndex)
```


Se prepara para procesar una celda.

**Remarks**

Se llamará al alcanzar una celda existente en la fila actual. La fila actual es la fila de la última llamada de [processRow(Row)](../../com.aspose.cells/lightcellsdatahandler\#processRow-Row-).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | int | índice de columna de la celda a procesar |

**Returns:**
booleano - indica si esta celda necesita ser procesada. false para ignorar la celda y comprobar la siguiente hasta alcanzar el final de los datos de celdas de la fila actual
### startRow(int rowIndex) {#startRow-int-}
```
public abstract boolean startRow(int rowIndex)
```


Se prepara para procesar una fila.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | int | el índice de la siguiente fila a procesar |

**Returns:**
booleano - indica si esta fila (propiedades o datos de celdas) necesita ser procesada. false para ignorar esta fila y sus celdas y comprobar la siguiente fila.
### startSheet(Worksheet sheet) {#startSheet-com.aspose.cells.Worksheet-}
```
public abstract boolean startSheet(Worksheet sheet)
```


Comienza a procesar una hoja de cálculo.

**Remarks**

Se llamará antes de leer los datos de celdas de una hoja de cálculo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheet | [Worksheet](../../com.aspose.cells/worksheet) | la hoja de cálculo de la que leer los datos de celdas. |

**Returns:**
booleano - indica si los datos de celdas de esta hoja necesitan ser procesados. false para ignorar esta hoja.
