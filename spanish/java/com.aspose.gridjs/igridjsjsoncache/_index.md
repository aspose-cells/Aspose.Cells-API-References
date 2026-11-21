---
title: "IGridJsJsonCache"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Interfaz de caché JSON - los clientes implementan estrategias específicas de almacenamiento e invalidación"
type: docs
url: /es/java/com.aspose.gridjs/igridjsjsoncache/
---
```
public interface IGridJsJsonCache
```

Interfaz de caché JSON - los clientes implementan estrategias específicas de almacenamiento e invalidación
## Métodos

| Método | Descripción |
| --- | --- |
| [clearAll()](#clearAll--) | Borrar todas las cachés |
| [getCacheKey(String uid, String fileName)](#getCacheKey-java.lang.String-java.lang.String-) | Genera una clave de caché. |
| [invalidate(String cacheKey)](#invalidate-java.lang.String-) | Invalidar la entrada de caché especificada. |
| [invalidateAllForUid(String uid)](#invalidateAllForUid-java.lang.String-) | Invalidar todas las entradas de caché que contengan el uid especificado. |
| [setJson(String cacheKey, String json)](#setJson-java.lang.String-java.lang.String-) | Escribir JSON en la caché. |
| [tryGetJson(String cacheKey)](#tryGetJson-java.lang.String-) | Intentar recuperar JSON de la caché. |
### clearAll() {#clearAll--}
```
public abstract void clearAll()
```


Borrar todas las cachés

### getCacheKey(String uid, String fileName) {#getCacheKey-java.lang.String-java.lang.String-}
```
public abstract String getCacheKey(String uid, String fileName)
```


Generar una clave de caché. Los clientes pueden decidir si incluir el uid según los requisitos del negocio. - Si solo importa el nombre del archivo: ignore el uid y use solo fileName (recomendado, permite compartir la caché entre el mismo archivo). - Si se requiere distinguir archivos con el mismo nombre: use uid (modo estricto).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| uid | java.lang.String | Identificador único del archivo (puede variar por carga). |
| fileName | java.lang.String | Nombre de archivo original |

**Returns:**
java.lang.String - Cache key
### invalidate(String cacheKey) {#invalidate-java.lang.String-}
```
public abstract void invalidate(String cacheKey)
```


Invalidar la entrada de caché especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cacheKey | java.lang.String | Clave de caché |

### invalidateAllForUid(String uid) {#invalidateAllForUid-java.lang.String-}
```
public abstract void invalidateAllForUid(String uid)
```


Invalidar todas las entradas de caché que contengan el uid especificado. Esto es útil cuando no sabes el fileName exacto utilizado para la caché.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| uid | java.lang.String | Identificador único para coincidir en las claves de caché |

### setJson(String cacheKey, String json) {#setJson-java.lang.String-java.lang.String-}
```
public abstract void setJson(String cacheKey, String json)
```


Escribir JSON en la caché.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cacheKey | java.lang.String | Clave de caché |
| json | java.lang.String | cadena JSON |

### tryGetJson(String cacheKey) {#tryGetJson-java.lang.String-}
```
public abstract String tryGetJson(String cacheKey)
```


Intentar recuperar JSON de la caché.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cacheKey | java.lang.String | Clave de caché |

**Returns:**
java.lang.String - cadena JSON si hay coincidencia en caché, null de lo contrario
