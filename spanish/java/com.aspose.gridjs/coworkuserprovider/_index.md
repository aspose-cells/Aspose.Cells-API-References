---
title: "CoWorkUserProvider"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa la interfaz del proveedor de usuarios en modo de colaboración. solo disponible en la versión java ahora, estará disponible en la versión .netython en el futuro."
type: docs
url: /es/java/com.aspose.gridjs/coworkuserprovider/
---
```
public interface CoWorkUserProvider
```

Representa la interfaz del proveedor de usuarios en modo de colaboración. solo disponible en la versión java ahora, estará disponible en la versión .net/python en el futuro. La aplicación cliente puede implementar esta interfaz para proporcionar la información del usuario.
## Métodos

| Método | Descripción |
| --- | --- |
| [getCurrentUserId()](#getCurrentUserId--) | Obtiene el identificador único del usuario actual |
| [getCurrentUserName()](#getCurrentUserName--) | Obtiene el nombre de usuario del usuario actual |
| [getPermission()](#getPermission--) | Obtiene el nivel de permiso del usuario actual |
### getCurrentUserId() {#getCurrentUserId--}
```
public abstract long getCurrentUserId()
```


Obtiene el identificador único del usuario actual

**Returns:**
long - ID de usuario actual
### getCurrentUserName() {#getCurrentUserName--}
```
public abstract String getCurrentUserName()
```


Obtiene el nombre de usuario del usuario actual

**Returns:**
java.lang.String - Nombre de usuario actual
### getPermission() {#getPermission--}
```
public abstract int getPermission()
```


Obtiene el nivel de permiso del usuario actual

**Returns:**
int - [CoWorkUserPermission](../../com.aspose.gridjs/coworkuserpermission). Nivel de permiso del usuario actual
