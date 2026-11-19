---
title: "CoWorkUserProvider"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente l'interface du fournisseur d'utilisateur en mode collaboration. uniquement disponible dans la version java pour le moment, sera disponible dans la version .netython à l'avenir."
type: docs
url: /fr/java/com.aspose.gridjs/coworkuserprovider/
---
```
public interface CoWorkUserProvider
```

Représente l'interface du fournisseur d'utilisateur en mode collaboration. uniquement disponible dans la version java pour le moment, sera disponible dans la version .net/python à l'avenir. L'application cliente peut implémenter cette interface pour fournir les informations utilisateur.
## Méthodes

| Méthode | Description |
| --- | --- |
| [getCurrentUserId()](#getCurrentUserId--) | Obtient l'identifiant unique de l'utilisateur actuel |
| [getCurrentUserName()](#getCurrentUserName--) | Obtient le nom d'utilisateur de l'utilisateur actuel |
| [getPermission()](#getPermission--) | Obtient le niveau d'autorisation de l'utilisateur actuel |
### getCurrentUserId() {#getCurrentUserId--}
```
public abstract long getCurrentUserId()
```


Obtient l'identifiant unique de l'utilisateur actuel

**Returns:**
long - ID utilisateur actuel
### getCurrentUserName() {#getCurrentUserName--}
```
public abstract String getCurrentUserName()
```


Obtient le nom d'utilisateur de l'utilisateur actuel

**Returns:**
java.lang.String - Nom d'utilisateur actuel
### getPermission() {#getPermission--}
```
public abstract int getPermission()
```


Obtient le niveau d'autorisation de l'utilisateur actuel

**Returns:**
int - [CoWorkUserPermission](../../com.aspose.gridjs/coworkuserpermission). Niveau d'autorisation actuel de l'utilisateur
