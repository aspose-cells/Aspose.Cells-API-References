---
title: "ISmartMarkerCallBack"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa la interfaz de devolución de llamada del procesamiento de smartmarker."
type: docs
url: /es/java/com.aspose.cells/ismartmarkercallback/
---
```
public interface ISmartMarkerCallBack
```

Representa la interfaz de devolución de llamada del procesamiento de smartmarker.
## Métodos

| Método | Descripción |
| --- | --- |
| [process(int sheetIndex, int rowIndex, int colIndex, String tableName, String columnName)](#process-int-int-int-java.lang.String-java.lang.String-) | Función de devolución de llamada para procesar un marcador inteligente. |
### process(int sheetIndex, int rowIndex, int colIndex, String tableName, String columnName) {#process-int-int-int-java.lang.String-java.lang.String-}
```
public abstract void process(int sheetIndex, int rowIndex, int colIndex, String tableName, String columnName)
```


Función de devolución de llamada para procesar un marcador inteligente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetIndex | int | El índice de la hoja. |
| rowIndex | int | El índice de fila. |
| colIndex | int | El índice de columna. |
| tableName | java.lang.String | El nombre de tabla del marcador inteligente. |
| columnName | java.lang.String | El nombre de tabla del marcador inteligente. |

