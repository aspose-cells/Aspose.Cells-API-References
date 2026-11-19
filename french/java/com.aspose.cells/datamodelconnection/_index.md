---
title: "DataModelConnection"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Spécifie une connexion au modèle de données"
type: docs
url: /fr/java/com.aspose.cells/datamodelconnection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ExternalConnection](../../com.aspose.cells/externalconnection)
```
public class DataModelConnection extends ExternalConnection
```

Spécifie une connexion au modèle de données
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackgroundRefresh()](#getBackgroundRefresh--) | Indique si la connexion peut être rafraîchie en arrière-plan (asynchroniquement). |
| [getClass()](#getClass--) |  |
| [getClassType()](#getClassType--) | Obtient le type de cet objet [ExternalConnection](../../com.aspose.cells/externalconnection). |
| [getCommand()](#getCommand--) | La chaîne contenant la commande de base de données à transmettre à l'API du fournisseur de données qui interagira avec la source externe afin de récupérer les données. |
| [getCommandType()](#getCommandType--) | Renvoie le type [OLEDBCommandType](../../com.aspose.cells/oledbcommandtype). |
| [getConnectionDescription()](#getConnectionDescription--) | Spécifie la description utilisateur pour cette connexion. |
| [getConnectionFile()](#getConnectionFile--) | Obtient le fichier de connexion. |
| [getConnectionId()](#getConnectionId--) | Spécifie l'identifiant unique de cette connexion. |
| [getConnectionString()](#getConnectionString--) | La chaîne d'informations de connexion est utilisée pour établir le contact avec une source de données OLE DB ou ODBC. |
| [getCredentials()](#getCredentials--) | Spécifie la méthode d'authentification à utiliser lors de l'établissement (ou du rétablissement) de la connexion. |
| [getCredentialsMethodType()](#getCredentialsMethodType--) | Spécifie la méthode d'authentification à utiliser lors de l'établissement (ou du rétablissement) de la connexion. |
| [getId()](#getId--) | Obtient l'ID de la connexion. |
| [getKeepAlive()](#getKeepAlive--) | Vrai lorsque l'application de feuille de calcul doit faire des efforts pour maintenir la connexion ouverte. |
| [getName()](#getName--) | Spécifie le nom de la connexion. |
| [getOdcFile()](#getOdcFile--) | Spécifie le chemin complet du fichier de connexion externe à partir duquel cette connexion a été créée. |
| [getOnlyUseConnectionFile()](#getOnlyUseConnectionFile--) | Indique si l'application de feuille de calcul doit toujours et uniquement utiliser les informations de connexion du fichier de connexion externe indiqué par l'attribut odcFile lors du rafraîchissement de la connexion. |
| [getParameters()](#getParameters--) | Obtient [ConnectionParameterCollection](../../com.aspose.cells/connectionparametercollection) pour une requête ODBC ou web. |
| [getPowerQueryFormula()](#getPowerQueryFormula--) | Obtient la définition de la formule Power Query. |
| [getReconnectionMethod()](#getReconnectionMethod--) | Spécifie ce que l'application de feuille de calcul doit faire lorsqu'une connexion échoue. |
| [getReconnectionMethodType()](#getReconnectionMethodType--) | Spécifie ce que l'application de feuille de calcul doit faire lorsqu'une connexion échoue. |
| [getRefreshInternal()](#getRefreshInternal--) | Spécifie le nombre de minutes entre les rafraîchissements automatiques de la connexion. |
| [getRefreshOnLoad()](#getRefreshOnLoad--) | Vrai si cette connexion doit être rafraîchie lors de l'ouverture du fichier ; sinon, faux. |
| [getSSOId()](#getSSOId--) | Identifiant pour l'authentification Single Sign On (SSO) utilisée entre un serveur intermédiaire spreadsheetML et la source de données externe. |
| [getSaveData()](#getSaveData--) | Vrai si les données externes récupérées via la connexion pour remplir un tableau doivent être enregistrées avec le classeur ; sinon, faux. |
| [getSavePassword()](#getSavePassword--) | Vrai si le mot de passe doit être enregistré dans la chaîne de connexion ; sinon, Faux. |
| [getSecondCommand()](#getSecondCommand--) | Spécifie une deuxième chaîne de texte de commande qui est conservée lorsque les champs de page basés sur le serveur PivotTable sont utilisés. |
| [getSourceFile()](#getSourceFile--) | Utilisé lorsque la source de données externe est basée sur un fichier. |
| [getSourceType()](#getSourceType--) | Obtient le type de DataSource de la connexion externe. |
| [getType()](#getType--) | Obtient le type de DataSource de la connexion externe. |
| [hashCode()](#hashCode--) |  |
| [isDeleted()](#isDeleted--) | Indique si la connexion du classeur associée a été supprimée. |
| [isNew()](#isNew--) | Vrai si la connexion n’a pas été actualisée pour la première fois ; sinon, faux. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackgroundRefresh(boolean value)](#setBackgroundRefresh-boolean-) | Indique si la connexion peut être rafraîchie en arrière-plan (asynchroniquement). |
| [setCommand(String value)](#setCommand-java.lang.String-) | La chaîne contenant la commande de base de données à transmettre à l'API du fournisseur de données qui interagira avec la source externe afin de récupérer les données. |
| [setCommandType(int value)](#setCommandType-int-) | Renvoie le type [OLEDBCommandType](../../com.aspose.cells/oledbcommandtype). |
| [setConnectionDescription(String value)](#setConnectionDescription-java.lang.String-) | Spécifie la description utilisateur pour cette connexion. |
| [setConnectionString(String value)](#setConnectionString-java.lang.String-) | La chaîne d'informations de connexion est utilisée pour établir le contact avec une source de données OLE DB ou ODBC. |
| [setCredentials(int value)](#setCredentials-int-) | Spécifie la méthode d'authentification à utiliser lors de l'établissement (ou du rétablissement) de la connexion. |
| [setCredentialsMethodType(int value)](#setCredentialsMethodType-int-) | Spécifie la méthode d'authentification à utiliser lors de l'établissement (ou du rétablissement) de la connexion. |
| [setDeleted(boolean value)](#setDeleted-boolean-) | Indique si la connexion du classeur associée a été supprimée. |
| [setKeepAlive(boolean value)](#setKeepAlive-boolean-) | Vrai lorsque l'application de feuille de calcul doit faire des efforts pour maintenir la connexion ouverte. |
| [setName(String value)](#setName-java.lang.String-) | Spécifie le nom de la connexion. |
| [setNew(boolean value)](#setNew-boolean-) | Vrai si la connexion n’a pas été actualisée pour la première fois ; sinon, faux. |
| [setOdcFile(String value)](#setOdcFile-java.lang.String-) | Spécifie le chemin complet du fichier de connexion externe à partir duquel cette connexion a été créée. |
| [setOnlyUseConnectionFile(boolean value)](#setOnlyUseConnectionFile-boolean-) | Indique si l'application de feuille de calcul doit toujours et uniquement utiliser les informations de connexion du fichier de connexion externe indiqué par l'attribut odcFile lors du rafraîchissement de la connexion. |
| [setReconnectionMethod(int value)](#setReconnectionMethod-int-) | Spécifie ce que l'application de feuille de calcul doit faire lorsqu'une connexion échoue. |
| [setReconnectionMethodType(int value)](#setReconnectionMethodType-int-) | Spécifie ce que l'application de feuille de calcul doit faire lorsqu'une connexion échoue. |
| [setRefreshInternal(int value)](#setRefreshInternal-int-) | Spécifie le nombre de minutes entre les rafraîchissements automatiques de la connexion. |
| [setRefreshOnLoad(boolean value)](#setRefreshOnLoad-boolean-) | Vrai si cette connexion doit être rafraîchie lors de l'ouverture du fichier ; sinon, faux. |
| [setSSOId(String value)](#setSSOId-java.lang.String-) | Identifiant pour l'authentification Single Sign On (SSO) utilisée entre un serveur intermédiaire spreadsheetML et la source de données externe. |
| [setSaveData(boolean value)](#setSaveData-boolean-) | Vrai si les données externes récupérées via la connexion pour remplir un tableau doivent être enregistrées avec le classeur ; sinon, faux. |
| [setSavePassword(boolean value)](#setSavePassword-boolean-) | Vrai si le mot de passe doit être enregistré dans la chaîne de connexion ; sinon, Faux. |
| [setSecondCommand(String value)](#setSecondCommand-java.lang.String-) | Spécifie une deuxième chaîne de texte de commande qui est conservée lorsque les champs de page basés sur le serveur PivotTable sont utilisés. |
| [setSourceFile(String value)](#setSourceFile-java.lang.String-) | Utilisé lorsque la source de données externe est basée sur un fichier. |
| [setSourceType(int value)](#setSourceType-int-) | Définit le type de DataSource de la connexion externe. |
| [setType(int value)](#setType-int-) | Définit le type de DataSource de la connexion externe. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getBackgroundRefresh() {#getBackgroundRefresh--}
```
public boolean getBackgroundRefresh()
```


Indique si la connexion peut être actualisée en arrière-plan (asynchroniquement). true si l’utilisation préférée de la connexion est de l’actualiser de façon asynchrone en arrière-plan ; false si l’utilisation préférée de la connexion est de l’actualiser de façon synchrone au premier plan.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getClassType() {#getClassType--}
```
public int getClassType()
```


Obtient le type de cet objet [ExternalConnection](../../com.aspose.cells/externalconnection).

Voir [ExternalConnectionClassType](../../com.aspose.cells/externalconnectionclasstype).

**Returns:**
int
### getCommand() {#getCommand--}
```
public String getCommand()
```


La chaîne contenant la commande de base de données à transmettre à l'API du fournisseur de données qui interagira avec la source externe afin de récupérer les données.

**Returns:**
java.lang.String
### getCommandType() {#getCommandType--}
```
public int getCommandType()
```


Renvoie le type [OLEDBCommandType](../../com.aspose.cells/oledbcommandtype).

Voir [OLEDBCommandType](../../com.aspose.cells/oledbcommandtype).

**Returns:**
int
### getConnectionDescription() {#getConnectionDescription--}
```
public String getConnectionDescription()
```


Spécifie la description utilisateur pour cette connexion.

**Returns:**
java.lang.String
### getConnectionFile() {#getConnectionFile--}
```
public String getConnectionFile()
```


Obtient le fichier de connexion.

**Returns:**
java.lang.String
### getConnectionId() {#getConnectionId--}
```
public int getConnectionId()
```


Spécifie l'identifiant unique de cette connexion.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. Veuillez plutôt utiliser la propriété ExternalConnection.Id. Cette propriété sera supprimée 12 mois après octobre 2024. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
int
### getConnectionString() {#getConnectionString--}
```
public String getConnectionString()
```


La chaîne d'informations de connexion est utilisée pour établir le contact avec une source de données OLE DB ou ODBC.

**Returns:**
java.lang.String
### getCredentials() {#getCredentials--}
```
public int getCredentials()
```


Spécifie la méthode d'authentification à utiliser lors de l'établissement (ou du rétablissement) de la connexion.

Voir [CredentialsMethodType](../../com.aspose.cells/credentialsmethodtype).

**Remarks**

NOTE : Cette propriété est maintenant obsolète. Veuillez plutôt utiliser la propriété ExternalConnection.CredentialsMethodType. Cette propriété sera supprimée 12 mois après octobre 2017. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
int
### getCredentialsMethodType() {#getCredentialsMethodType--}
```
public int getCredentialsMethodType()
```


Spécifie la méthode d'authentification à utiliser lors de l'établissement (ou du rétablissement) de la connexion.

Voir [CredentialsMethodType](../../com.aspose.cells/credentialsmethodtype).

**Returns:**
int
### getId() {#getId--}
```
public int getId()
```


Obtient l'ID de la connexion.

**Returns:**
int
### getKeepAlive() {#getKeepAlive--}
```
public boolean getKeepAlive()
```


Vrai lorsque l’application de feuille de calcul doit faire des efforts pour maintenir la connexion ouverte. Lorsque faux, l’application doit fermer la connexion après avoir récupéré les informations.

**Returns:**
boolean
### getName() {#getName--}
```
public String getName()
```


Spécifie le nom de la connexion. Chaque connexion doit avoir un nom unique.

**Returns:**
java.lang.String
### getOdcFile() {#getOdcFile--}
```
public String getOdcFile()
```


Spécifie le chemin complet vers le fichier de connexion externe à partir duquel cette connexion a été créée. Si une connexion échoue lors d’une tentative d’actualisation des données, et que reconnectionMethod=1, l’application de feuille de calcul réessaiera en utilisant les informations du fichier de connexion externe plutôt que l’objet de connexion intégré au classeur.

**Returns:**
java.lang.String
### getOnlyUseConnectionFile() {#getOnlyUseConnectionFile--}
```
public boolean getOnlyUseConnectionFile()
```


Indique si l’application de feuille de calcul doit toujours et uniquement utiliser les informations de connexion du fichier de connexion externe indiqué par l’attribut odcFile lors de l’actualisation de la connexion. Si faux, l’application de feuille de calcul doit suivre la procédure indiquée par l’attribut reconnectionMethod.

**Returns:**
boolean
### getParameters() {#getParameters--}
```
public ConnectionParameterCollection getParameters()
```


Obtient [ConnectionParameterCollection](../../com.aspose.cells/connectionparametercollection) pour une requête ODBC ou web.

**Returns:**
[ConnectionParameterCollection](../../com.aspose.cells/connectionparametercollection)
### getPowerQueryFormula() {#getPowerQueryFormula--}
```
public PowerQueryFormula getPowerQueryFormula()
```


Obtient la définition de la formule Power Query.

**Returns:**
[PowerQueryFormula](../../com.aspose.cells/powerqueryformula)
### getReconnectionMethod() {#getReconnectionMethod--}
```
public int getReconnectionMethod()
```


Spécifie ce que l’application de feuille de calcul doit faire lorsqu’une connexion échoue. La valeur par défaut est ReConnectionMethodType.Required.

Voir [ReConnectionMethodType](../../com.aspose.cells/reconnectionmethodtype).

**Remarks**

NOTE : Cette propriété est maintenant obsolète. Veuillez plutôt utiliser la propriété ExternalConnection.ReconnectionMethodType. Cette propriété sera supprimée 12 mois après octobre 2017. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
int
### getReconnectionMethodType() {#getReconnectionMethodType--}
```
public int getReconnectionMethodType()
```


Spécifie ce que l’application de feuille de calcul doit faire lorsqu’une connexion échoue. La valeur par défaut est ReConnectionMethodType.Required.

Voir [ReConnectionMethodType](../../com.aspose.cells/reconnectionmethodtype).

**Returns:**
int
### getRefreshInternal() {#getRefreshInternal--}
```
public int getRefreshInternal()
```


Spécifie le nombre de minutes entre les rafraîchissements automatiques de la connexion.

**Returns:**
int
### getRefreshOnLoad() {#getRefreshOnLoad--}
```
public boolean getRefreshOnLoad()
```


Vrai si cette connexion doit être rafraîchie lors de l'ouverture du fichier ; sinon, faux.

**Returns:**
boolean
### getSSOId() {#getSSOId--}
```
public String getSSOId()
```


Identifiant pour l'authentification Single Sign On (SSO) utilisée entre un serveur intermédiaire spreadsheetML et la source de données externe.

**Returns:**
java.lang.String
### getSaveData() {#getSaveData--}
```
public boolean getSaveData()
```


Vrai si les données externes récupérées via la connexion pour remplir un tableau doivent être enregistrées avec le classeur ; sinon, faux.

**Returns:**
boolean
### getSavePassword() {#getSavePassword--}
```
public boolean getSavePassword()
```


Vrai si le mot de passe doit être enregistré dans la chaîne de connexion ; sinon, Faux.

**Returns:**
boolean
### getSecondCommand() {#getSecondCommand--}
```
public String getSecondCommand()
```


Spécifie une deuxième chaîne de texte de commande qui est conservée lorsque des champs de page de tableau croisé dynamique basés sur le serveur sont utilisés. Pour les connexions ODBC, serverCommand est généralement une requête plus large que command (aucune clause WHERE n’est présente dans la première). En se basant sur ces 2 commandes (Command et ServerCommand), l’interface utilisateur des paramètres peut être remplie et des requêtes paramétrées peuvent être construites.

**Returns:**
java.lang.String
### getSourceFile() {#getSourceFile--}
```
public String getSourceFile()
```


Utilisé lorsque la source de données externe est basée sur un fichier. Lorsqu’une connexion à une telle source de données échoue, l’application de feuille de calcul tente de se connecter directement à ce fichier. Peut être exprimé sous forme d’URI ou de notation de chemin de fichier spécifique au système.

**Returns:**
java.lang.String
### getSourceType() {#getSourceType--}
```
public int getSourceType()
```


Obtient le type de DataSource de la connexion externe.

Voir [ConnectionDataSourceType](../../com.aspose.cells/connectiondatasourcetype).

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Obtient le type de DataSource de la connexion externe.

Voir [ConnectionDataSourceType](../../com.aspose.cells/connectiondatasourcetype).

**Remarks**

NOTE: Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété ExternalConnection.SourceType. Cette propriété sera supprimée 12 mois plus tard à compter d’octobre 2024. Aspose s’excuse pour tout désagrément que vous avez pu rencontrer.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isDeleted() {#isDeleted--}
```
public boolean isDeleted()
```


Indique si la connexion de classeur associée a été supprimée. true si la connexion a été supprimée ; sinon, false.

**Returns:**
boolean
### isNew() {#isNew--}
```
public boolean isNew()
```


True si la connexion n’a pas été rafraîchie pour la première fois ; sinon, false. Cet état peut se produire lorsque l’utilisateur enregistre le fichier avant qu’une requête ne soit terminée.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setBackgroundRefresh(boolean value) {#setBackgroundRefresh-boolean-}
```
public void setBackgroundRefresh(boolean value)
```


Indique si la connexion peut être actualisée en arrière-plan (asynchroniquement). true si l’utilisation préférée de la connexion est de l’actualiser de façon asynchrone en arrière-plan ; false si l’utilisation préférée de la connexion est de l’actualiser de façon synchrone au premier plan.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setCommand(String value) {#setCommand-java.lang.String-}
```
public void setCommand(String value)
```


La chaîne contenant la commande de base de données à transmettre à l'API du fournisseur de données qui interagira avec la source externe afin de récupérer les données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setCommandType(int value) {#setCommandType-int-}
```
public void setCommandType(int value)
```


Renvoie le type [OLEDBCommandType](../../com.aspose.cells/oledbcommandtype).

Voir [OLEDBCommandType](../../com.aspose.cells/oledbcommandtype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setConnectionDescription(String value) {#setConnectionDescription-java.lang.String-}
```
public void setConnectionDescription(String value)
```


Spécifie la description utilisateur pour cette connexion.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setConnectionString(String value) {#setConnectionString-java.lang.String-}
```
public void setConnectionString(String value)
```


La chaîne d'informations de connexion est utilisée pour établir le contact avec une source de données OLE DB ou ODBC.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setCredentials(int value) {#setCredentials-int-}
```
public void setCredentials(int value)
```


Spécifie la méthode d'authentification à utiliser lors de l'établissement (ou du rétablissement) de la connexion.

Voir [CredentialsMethodType](../../com.aspose.cells/credentialsmethodtype).

**Remarks**

NOTE : Cette propriété est maintenant obsolète. Veuillez plutôt utiliser la propriété ExternalConnection.CredentialsMethodType. Cette propriété sera supprimée 12 mois après octobre 2017. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setCredentialsMethodType(int value) {#setCredentialsMethodType-int-}
```
public void setCredentialsMethodType(int value)
```


Spécifie la méthode d'authentification à utiliser lors de l'établissement (ou du rétablissement) de la connexion.

Voir [CredentialsMethodType](../../com.aspose.cells/credentialsmethodtype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setDeleted(boolean value) {#setDeleted-boolean-}
```
public void setDeleted(boolean value)
```


Indique si la connexion de classeur associée a été supprimée. true si la connexion a été supprimée ; sinon, false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setKeepAlive(boolean value) {#setKeepAlive-boolean-}
```
public void setKeepAlive(boolean value)
```


Vrai lorsque l’application de feuille de calcul doit faire des efforts pour maintenir la connexion ouverte. Lorsque faux, l’application doit fermer la connexion après avoir récupéré les informations.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Spécifie le nom de la connexion. Chaque connexion doit avoir un nom unique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setNew(boolean value) {#setNew-boolean-}
```
public void setNew(boolean value)
```


True si la connexion n’a pas été rafraîchie pour la première fois ; sinon, false. Cet état peut se produire lorsque l’utilisateur enregistre le fichier avant qu’une requête ne soit terminée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setOdcFile(String value) {#setOdcFile-java.lang.String-}
```
public void setOdcFile(String value)
```


Spécifie le chemin complet vers le fichier de connexion externe à partir duquel cette connexion a été créée. Si une connexion échoue lors d’une tentative d’actualisation des données, et que reconnectionMethod=1, l’application de feuille de calcul réessaiera en utilisant les informations du fichier de connexion externe plutôt que l’objet de connexion intégré au classeur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setOnlyUseConnectionFile(boolean value) {#setOnlyUseConnectionFile-boolean-}
```
public void setOnlyUseConnectionFile(boolean value)
```


Indique si l’application de feuille de calcul doit toujours et uniquement utiliser les informations de connexion du fichier de connexion externe indiqué par l’attribut odcFile lors de l’actualisation de la connexion. Si faux, l’application de feuille de calcul doit suivre la procédure indiquée par l’attribut reconnectionMethod.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setReconnectionMethod(int value) {#setReconnectionMethod-int-}
```
public void setReconnectionMethod(int value)
```


Spécifie ce que l’application de feuille de calcul doit faire lorsqu’une connexion échoue. La valeur par défaut est ReConnectionMethodType.Required.

Voir [ReConnectionMethodType](../../com.aspose.cells/reconnectionmethodtype).

**Remarks**

NOTE : Cette propriété est maintenant obsolète. Veuillez plutôt utiliser la propriété ExternalConnection.ReconnectionMethodType. Cette propriété sera supprimée 12 mois après octobre 2017. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setReconnectionMethodType(int value) {#setReconnectionMethodType-int-}
```
public void setReconnectionMethodType(int value)
```


Spécifie ce que l’application de feuille de calcul doit faire lorsqu’une connexion échoue. La valeur par défaut est ReConnectionMethodType.Required.

Voir [ReConnectionMethodType](../../com.aspose.cells/reconnectionmethodtype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setRefreshInternal(int value) {#setRefreshInternal-int-}
```
public void setRefreshInternal(int value)
```


Spécifie le nombre de minutes entre les rafraîchissements automatiques de la connexion.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setRefreshOnLoad(boolean value) {#setRefreshOnLoad-boolean-}
```
public void setRefreshOnLoad(boolean value)
```


Vrai si cette connexion doit être rafraîchie lors de l'ouverture du fichier ; sinon, faux.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSSOId(String value) {#setSSOId-java.lang.String-}
```
public void setSSOId(String value)
```


Identifiant pour l'authentification Single Sign On (SSO) utilisée entre un serveur intermédiaire spreadsheetML et la source de données externe.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setSaveData(boolean value) {#setSaveData-boolean-}
```
public void setSaveData(boolean value)
```


Vrai si les données externes récupérées via la connexion pour remplir un tableau doivent être enregistrées avec le classeur ; sinon, faux.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSavePassword(boolean value) {#setSavePassword-boolean-}
```
public void setSavePassword(boolean value)
```


Vrai si le mot de passe doit être enregistré dans la chaîne de connexion ; sinon, Faux.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSecondCommand(String value) {#setSecondCommand-java.lang.String-}
```
public void setSecondCommand(String value)
```


Spécifie une deuxième chaîne de texte de commande qui est conservée lorsque des champs de page de tableau croisé dynamique basés sur le serveur sont utilisés. Pour les connexions ODBC, serverCommand est généralement une requête plus large que command (aucune clause WHERE n’est présente dans la première). En se basant sur ces 2 commandes (Command et ServerCommand), l’interface utilisateur des paramètres peut être remplie et des requêtes paramétrées peuvent être construites.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setSourceFile(String value) {#setSourceFile-java.lang.String-}
```
public void setSourceFile(String value)
```


Utilisé lorsque la source de données externe est basée sur un fichier. Lorsqu’une connexion à une telle source de données échoue, l’application de feuille de calcul tente de se connecter directement à ce fichier. Peut être exprimé sous forme d’URI ou de notation de chemin de fichier spécifique au système.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setSourceType(int value) {#setSourceType-int-}
```
public void setSourceType(int value)
```


Définit le type de DataSource de la connexion externe.

Voir [ConnectionDataSourceType](../../com.aspose.cells/connectiondatasourcetype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Définit le type de DataSource de la connexion externe.

Voir [ConnectionDataSourceType](../../com.aspose.cells/connectiondatasourcetype).

**Remarks**

NOTE: Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété ExternalConnection.SourceType. Cette propriété sera supprimée 12 mois plus tard à compter d’octobre 2024. Aspose s’excuse pour tout désagrément que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

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

