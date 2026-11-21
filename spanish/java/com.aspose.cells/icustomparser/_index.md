---
title: "ICustomParser"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Permite a los usuarios agregar su analizador de valores personalizado para convertir valores de cadena a otro objeto de valor de celda adecuado."
type: docs
url: /es/java/com.aspose.cells/icustomparser/
---
```
public interface ICustomParser
```

Permite a los usuarios agregar su analizador de valores personalizado para convertir valores de cadena a otro objeto de valor de celda adecuado.
## Métodos

| Método | Descripción |
| --- | --- |
| [getFormat()](#getFormat--) | Obtiene el patrón de formato correspondiente al valor analizado por la última invocación de [parseObject(String)](../../com.aspose.cells/icustomparser\#parseObject-String-). |
| [parseObject(String value)](#parseObject-java.lang.String-) | Analiza la cadena proporcionada a un objeto de valor adecuado. |
### getFormat() {#getFormat--}
```
public abstract String getFormat()
```


Obtiene el patrón de formato correspondiente al valor analizado por la última invocación de [parseObject(String)](../../com.aspose.cells/icustomparser\#parseObject-String-).

**Remarks**

El patrón de formato devuelto puede usarse para formatear la celda correspondiente (establezca Style.Custom para la celda).

**Returns:**
java.lang.String
### parseObject(String value) {#parseObject-java.lang.String-}
```
public abstract Object parseObject(String value)
```


Analiza la cadena proporcionada a un objeto de valor adecuado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | El valor de cadena a analizar |

**Returns:**
java.lang.Object - Objeto de valor analizado a partir de la cadena proporcionada. Si la cadena dada no puede analizarse a un objeto de valor adecuado, devuelve null.
