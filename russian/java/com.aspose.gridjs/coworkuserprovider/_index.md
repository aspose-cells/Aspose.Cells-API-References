---
title: "CoWorkUserProvider"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет интерфейс поставщика пользователей в режиме совместной работы. Сейчас доступен только в версии Java, в будущем будет доступен в версии .NET/Python."
type: docs
url: /ru/java/com.aspose.gridjs/coworkuserprovider/
---
```
public interface CoWorkUserProvider
```

Представляет интерфейс поставщика пользователей в режиме совместной работы. Сейчас доступен только в версии Java, в будущем будет доступен в версии .NET/Python. Приложение‑клиент может реализовать этот интерфейс для предоставления информации о пользователе.
## Методы

| Метод | Описание |
| --- | --- |
| [getCurrentUserId()](#getCurrentUserId--) | Получает уникальный идентификатор текущего пользователя |
| [getCurrentUserName()](#getCurrentUserName--) | Получает имя пользователя текущего пользователя |
| [getPermission()](#getPermission--) | Получает уровень разрешений текущего пользователя |
### getCurrentUserId() {#getCurrentUserId--}
```
public abstract long getCurrentUserId()
```


Получает уникальный идентификатор текущего пользователя

**Returns:**
long — идентификатор текущего пользователя
### getCurrentUserName() {#getCurrentUserName--}
```
public abstract String getCurrentUserName()
```


Получает имя пользователя текущего пользователя

**Returns:**
java.lang.String — имя текущего пользователя
### getPermission() {#getPermission--}
```
public abstract int getPermission()
```


Получает уровень разрешений текущего пользователя

**Returns:**
int — [CoWorkUserPermission](../../com.aspose.gridjs/coworkuserpermission). Текущий уровень разрешений пользователя
