---
title: "GridCustomServerValidation"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "La interfaz que necesitas implementar al usar validación del lado del servidor."
type: docs
url: /es/java/com.aspose.gridweb/gridcustomservervalidation/
---
```
public interface GridCustomServerValidation
```

la interfaz que necesitas implementar al usar validación del lado del servidor. CustomServerFunction.
## Métodos

| Método | Descripción |
| --- | --- |
| [validate(GridWorksheet sheet, int row, int col, String value)](#validate-com.aspose.gridweb.GridWorksheet-int-int-java.lang.String-) | **Observaciones** |
### validate(GridWorksheet sheet, int row, int col, String value) {#validate-com.aspose.gridweb.GridWorksheet-int-int-java.lang.String-}
```
public abstract String validate(GridWorksheet sheet, int row, int col, String value)
```


**Remarks**

si devuelve string.empty la validación pasa, de lo contrario puedes devolver cualquier mensaje relacionado que pueda ser manejado en la función ClientCallback.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheet | [GridWorksheet](../../com.aspose.gridweb/gridworksheet) | el GridWorksheet |
| fila | int | el índice de fila de la celda |
| col | int | el índice de columna de la celda |
| valor | java.lang.String | el valor para realizar la validación |

**Returns:**
java.lang.String - valor de resultado basado en cadena
