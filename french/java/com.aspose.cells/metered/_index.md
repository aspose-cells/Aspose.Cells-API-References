---
title: "Mesuré"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Fournit des méthodes pour définir la clé mesurée."
type: docs
url: /fr/java/com.aspose.cells/metered/
---

**Inheritance:**
java.lang.Object
```
public class Metered
```

Fournit des méthodes pour définir la clé mesurée.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [Metered()](#Metered--) | Initialise une nouvelle instance de cette classe. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getConsumptionCredit()](#getConsumptionCredit--) | Obtient le crédit de consommation |
| [getConsumptionQuantity()](#getConsumptionQuantity--) | Obtient la taille du fichier de consommation |
| [getProductName()](#getProductName--) | Obtient le nom du produit |
| [hashCode()](#hashCode--) |  |
| [isMeteredLicensed()](#isMeteredLicensed--) | Vérifier si le metered est licencié |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | Définit la clé publique et privée du metered. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Metered() {#Metered--}
```
public Metered()
```


Initialise une nouvelle instance de cette classe.

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
### getConsumptionCredit() {#getConsumptionCredit--}
```
public static double getConsumptionCredit()
```


Obtient le crédit de consommation

**Returns:**
double - quantité de consommation
### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static double getConsumptionQuantity()
```


Obtient la taille du fichier de consommation

**Returns:**
double - quantité de consommation
### getProductName() {#getProductName--}
```
public String getProductName()
```


Obtient le nom du produit

**Returns:**
java.lang.String - nom du produit
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isMeteredLicensed() {#isMeteredLicensed--}
```
public static boolean isMeteredLicensed()
```


Vérifier si le metered est licencié

**Returns:**
boolean - vrai ou faux
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public void setMeteredKey(String publicKey, String privateKey)
```


Définit la clé publique et privée du metered. Si vous achetez une licence metered, au démarrage de l'application, cette API doit être appelée, normalement cela suffit. Cependant, si le téléchargement des données de consommation échoue constamment et dépasse 24 heures, la licence sera mise en statut d'évaluation ; pour éviter ce cas, vous devez vérifier régulièrement le statut de la licence, et s'il est en statut d'évaluation, appeler à nouveau cette API.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| publicKey | java.lang.String | clé publique |
| privateKey | java.lang.String | clé privée |

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

