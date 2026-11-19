---
title: "ReConnectionMethodType"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Spécifie ce que l'application de feuille de calcul doit faire lorsqu'une connexion échoue."
type: docs
url: /fr/java/com.aspose.cells/reconnectionmethodtype/
---

**Inheritance:**
java.lang.Object
```
public final class ReConnectionMethodType
```

Spécifie ce que l'application de feuille de calcul doit faire lorsqu'une connexion échoue.
## Champs

| Champ | Description |
| --- | --- |
| [ALWAYS](#ALWAYS) | À chaque actualisation, récupérez les informations de connexion mises à jour depuis le fichier de connexion externe, si disponible, et utilisez-les à la place des informations de connexion existantes. |
| [NEVER](#NEVER) | Ne jamais récupérer les informations de connexion mises à jour depuis le fichier de connexion externe, même s'il est disponible et même si les informations de connexion existantes sont invalides. |
| [REQUIRED](#REQUIRED) | Lors de l'actualisation, utilisez les informations de connexion existantes et, si elles s'avèrent invalides, récupérez alors les informations de connexion mises à jour, si elles sont disponibles dans le fichier de connexion externe. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ALWAYS {#ALWAYS}
```
public static final int ALWAYS
```


À chaque actualisation, récupérez les informations de connexion mises à jour depuis le fichier de connexion externe, si disponible, et utilisez-les à la place des informations de connexion existantes. Dans ce cas, le rafraîchissement des données échouera si le fichier de connexion externe est indisponible.

### NEVER {#NEVER}
```
public static final int NEVER
```


Ne jamais récupérer les informations de connexion mises à jour depuis le fichier de connexion externe, même s'il est disponible et même si les informations de connexion existantes sont invalides.

### REQUIRED {#REQUIRED}
```
public static final int REQUIRED
```


Lors de l'actualisation, utilisez les informations de connexion existantes et, si elles s'avèrent invalides, récupérez alors les informations de connexion mises à jour, si elles sont disponibles dans le fichier de connexion externe.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

