---
title: "IGridJsJsonCache"
second_title: "Справочник API Aspose.Cells for Java"
description: "Интерфейс кэша JSON — клиенты реализуют конкретные стратегии хранения и инвалидизации."
type: docs
url: /ru/java/com.aspose.gridjs/igridjsjsoncache/
---
```
public interface IGridJsJsonCache
```

Интерфейс кэша JSON — клиенты реализуют конкретные стратегии хранения и инвалидизации.
## Методы

| Метод | Описание |
| --- | --- |
| [clearAll()](#clearAll--) | Очистить все кэши |
| [getCacheKey(String uid, String fileName)](#getCacheKey-java.lang.String-java.lang.String-) | Создать ключ кэша. |
| [invalidate(String cacheKey)](#invalidate-java.lang.String-) | Аннулировать указанную запись кэша. |
| [invalidateAllForUid(String uid)](#invalidateAllForUid-java.lang.String-) | Аннулировать все записи кэша, содержащие указанный uid. |
| [setJson(String cacheKey, String json)](#setJson-java.lang.String-java.lang.String-) | Записать JSON в кэш. |
| [tryGetJson(String cacheKey)](#tryGetJson-java.lang.String-) | Попытка получить JSON из кэша. |
### clearAll() {#clearAll--}
```
public abstract void clearAll()
```


Очистить все кэши

### getCacheKey(String uid, String fileName) {#getCacheKey-java.lang.String-java.lang.String-}
```
public abstract String getCacheKey(String uid, String fileName)
```


Создать ключ кэша. Клиенты могут решить, включать ли uid в зависимости от бизнес‑требований. - Если важен только имя файла: игнорировать uid и использовать только fileName (рекомендовано, позволяет делиться кэшем между одинаковыми файлами). - Если необходимо различать файлы с одинаковым именем: использовать uid (строгий режим).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| uid | java.lang.String | Уникальный идентификатор файла (может различаться при каждой загрузке) |
| fileName | java.lang.String | Исходное имя файла |

**Returns:**
java.lang.String - Ключ кэша
### invalidate(String cacheKey) {#invalidate-java.lang.String-}
```
public abstract void invalidate(String cacheKey)
```


Аннулировать указанную запись кэша.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| cacheKey | java.lang.String | Ключ кэша |

### invalidateAllForUid(String uid) {#invalidateAllForUid-java.lang.String-}
```
public abstract void invalidateAllForUid(String uid)
```


Аннулировать все записи кэша, содержащие указанный uid. Это полезно, когда вы не знаете точное fileName, используемое для кэширования.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| uid | java.lang.String | Уникальный идентификатор для сопоставления в ключах кэша |

### setJson(String cacheKey, String json) {#setJson-java.lang.String-java.lang.String-}
```
public abstract void setJson(String cacheKey, String json)
```


Записать JSON в кэш.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| cacheKey | java.lang.String | Ключ кэша |
| json | java.lang.String | JSON-строка |

### tryGetJson(String cacheKey) {#tryGetJson-java.lang.String-}
```
public abstract String tryGetJson(String cacheKey)
```


Попытка получить JSON из кэша.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| cacheKey | java.lang.String | Ключ кэша |

**Returns:**
java.lang.String - JSON-строка при попадании в кэш, иначе null
