---
title: "IFilePathProvider"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa el proveedor de ruta de archivo exportado."
type: docs
url: /es/java/com.aspose.cells/ifilepathprovider/
---
```
public interface IFilePathProvider
```

Representa el proveedor de ruta de archivo exportado.
## Métodos

| Método | Descripción |
| --- | --- |
| [getFullName(String sheetName)](#getFullName-java.lang.String-) | Obtiene la ruta completa del archivo por nombre de Worksheet al exportar Worksheet a HTML por separado. |
### getFullName(String sheetName) {#getFullName-java.lang.String-}
```
public abstract String getFullName(String sheetName)
```


Obtiene la ruta completa del archivo por nombre de Worksheet al exportar Worksheet a HTML por separado. Así, las referencias entre los Worksheets pueden exportarse correctamente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetName | java.lang.String | Nombre de la hoja de cálculo |

**Returns:**
java.lang.String - la ruta completa del archivo
