---
title: "WebQueryConnection"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Spécifie les propriétés d'une source de requête web."
type: docs
url: /fr/java/com.aspose.cells/webqueryconnection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ExternalConnection](../../com.aspose.cells/externalconnection)
```
public class WebQueryConnection extends ExternalConnection
```

Spécifie les propriétés d'une source de requête Web. Une requête Web récupérera les données des tableaux HTML et peut également fournir des paramètres HTTP \"Get\" à traiter par le serveur Web lors de la génération du HTML en incluant les paramètres et les éléments de paramètres.
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackgroundRefresh()](#getBackgroundRefresh--) | Indique si la connexion peut être rafraîchie en arrière-plan (asynchroniquement). |
| [getClass()](#getClass--) |  |
| [getClassType()](#getClassType--) | Obtient le type de cet objet [ExternalConnection](../../com.aspose.cells/externalconnection). |
| [getCommand()](#getCommand--) | La chaîne contenant la commande de base de données à transmettre à l'API du fournisseur de données qui interagira avec la source externe afin de récupérer les données. |
| [getCommandType()](#getCommandType--) | Spécifie le type de commande OLE DB. 1. |
| [getConnectionDescription()](#getConnectionDescription--) | Spécifie la description utilisateur pour cette connexion. |
| [getConnectionFile()](#getConnectionFile--) | Obtient le fichier de connexion. |
| [getConnectionId()](#getConnectionId--) | Spécifie l'identifiant unique de cette connexion. |
| [getConnectionString()](#getConnectionString--) | La chaîne d'informations de connexion est utilisée pour établir le contact avec une source de données OLE DB ou ODBC. |
| [getCredentials()](#getCredentials--) | Spécifie la méthode d'authentification à utiliser lors de l'établissement (ou du rétablissement) de la connexion. |
| [getCredentialsMethodType()](#getCredentialsMethodType--) | Spécifie la méthode d'authentification à utiliser lors de l'établissement (ou du rétablissement) de la connexion. |
| [getEditPage()](#getEditPage--) | L'URL de la page Web destinée à l'utilisateur affichant les données de la requête Web. |
| [getEditWebPage()](#getEditWebPage--) | L'URL de la page Web destinée à l'utilisateur affichant les données de la requête Web. |
| [getHtmlFormat()](#getHtmlFormat--) | Comment gérer le formatage de la source HTML lors de l'importation des données de requête Web dans la feuille de calcul. |
| [getId()](#getId--) | Obtient l'ID de la connexion. |
| [getKeepAlive()](#getKeepAlive--) | Vrai lorsque l'application de feuille de calcul doit faire des efforts pour maintenir la connexion ouverte. |
| [getName()](#getName--) | Spécifie le nom de la connexion. |
| [getOdcFile()](#getOdcFile--) | Spécifie le chemin complet du fichier de connexion externe à partir duquel cette connexion a été créée. |
| [getOnlyUseConnectionFile()](#getOnlyUseConnectionFile--) | Indique si l'application de feuille de calcul doit toujours et uniquement utiliser les informations de connexion du fichier de connexion externe indiqué par l'attribut odcFile lors du rafraîchissement de la connexion. |
| [getParameters()](#getParameters--) | Obtient [ConnectionParameterCollection](../../com.aspose.cells/connectionparametercollection) pour une requête ODBC ou web. |
| [getPost()](#getPost--) | Renvoie ou définit la chaîne utilisée avec la méthode POST pour envoyer des données à un serveur Web afin de récupérer les données d'une requête Web. |
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
| [getUrl()](#getUrl--) | URL à utiliser pour actualiser les données externes. |
| [hashCode()](#hashCode--) |  |
| [isConsecutive()](#isConsecutive--) | Indicateur indiquant si les délimiteurs consécutifs doivent être traités comme un seul délimiteur. |
| [isDeleted()](#isDeleted--) | Indique si la connexion du classeur associée a été supprimée. |
| [isHtmlTables()](#isHtmlTables--) | Indicateur indiquant si les requêtes Web ne doivent fonctionner que sur les tableaux HTML. |
| [isNew()](#isNew--) | Vrai si la connexion n’a pas été actualisée pour la première fois ; sinon, faux. |
| [isParsePre()](#isParsePre--) | Indicateur indiquant si les données contenues dans les balises HTML PRE de la page Web sont analysées en colonnes lors de l'importation de la page dans une table de requête. |
| [isSameSettings()](#isSameSettings--) | Indicateur indiquant s'il faut analyser toutes les tables à l'intérieur d'un bloc PRE avec les mêmes paramètres de largeur que la première ligne. |
| [isTextDates()](#isTextDates--) | Indicateur indiquant si les dates doivent être importées dans les cellules de la feuille de calcul en tant que texte plutôt qu'en tant que dates. |
| [isXl2000()](#isXl2000--) | Ce drapeau existe pour assurer la compatibilité ascendante avec les anciens fichiers de feuille de calcul existants, et il est défini sur true si cette requête Web a été actualisée dans une application de feuille de calcul plus récente ou égale à Microsoft Excel 2000. |
| [isXl97()](#isXl97--) | Ce drapeau existe pour assurer la compatibilité ascendante avec les anciens fichiers de feuille de calcul existants, et il est défini sur true si cette requête Web a été créée dans Microsoft Excel 97. |
| [isXml()](#isXml--) | true si la source de la requête Web est XML (au lieu de HTML), sinon false. |
| [isXmlSourceData()](#isXmlSourceData--) | Drapeau indiquant que les données source XML doivent être importées au lieu du tableau HTML lui‑même. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackgroundRefresh(boolean value)](#setBackgroundRefresh-boolean-) | Indique si la connexion peut être rafraîchie en arrière-plan (asynchroniquement). |
| [setCommand(String value)](#setCommand-java.lang.String-) | La chaîne contenant la commande de base de données à transmettre à l'API du fournisseur de données qui interagira avec la source externe afin de récupérer les données. |
| [setCommandType(int value)](#setCommandType-int-) | Spécifie le type de commande OLE DB. 1. |
| [setConnectionDescription(String value)](#setConnectionDescription-java.lang.String-) | Spécifie la description utilisateur pour cette connexion. |
| [setConnectionString(String value)](#setConnectionString-java.lang.String-) | La chaîne d'informations de connexion est utilisée pour établir le contact avec une source de données OLE DB ou ODBC. |
| [setConsecutive(boolean value)](#setConsecutive-boolean-) | Indicateur indiquant si les délimiteurs consécutifs doivent être traités comme un seul délimiteur. |
| [setCredentials(int value)](#setCredentials-int-) | Spécifie la méthode d'authentification à utiliser lors de l'établissement (ou du rétablissement) de la connexion. |
| [setCredentialsMethodType(int value)](#setCredentialsMethodType-int-) | Spécifie la méthode d'authentification à utiliser lors de l'établissement (ou du rétablissement) de la connexion. |
| [setDeleted(boolean value)](#setDeleted-boolean-) | Indique si la connexion du classeur associée a été supprimée. |
| [setEditPage(String value)](#setEditPage-java.lang.String-) | L'URL de la page Web destinée à l'utilisateur affichant les données de la requête Web. |
| [setEditWebPage(String value)](#setEditWebPage-java.lang.String-) | L'URL de la page Web destinée à l'utilisateur affichant les données de la requête Web. |
| [setHtmlFormat(int value)](#setHtmlFormat-int-) | Comment gérer le formatage de la source HTML lors de l'importation des données de requête Web dans la feuille de calcul. |
| [setHtmlTables(boolean value)](#setHtmlTables-boolean-) | Indicateur indiquant si les requêtes Web ne doivent fonctionner que sur les tableaux HTML. |
| [setKeepAlive(boolean value)](#setKeepAlive-boolean-) | Vrai lorsque l'application de feuille de calcul doit faire des efforts pour maintenir la connexion ouverte. |
| [setName(String value)](#setName-java.lang.String-) | Spécifie le nom de la connexion. |
| [setNew(boolean value)](#setNew-boolean-) | Vrai si la connexion n’a pas été actualisée pour la première fois ; sinon, faux. |
| [setOdcFile(String value)](#setOdcFile-java.lang.String-) | Spécifie le chemin complet du fichier de connexion externe à partir duquel cette connexion a été créée. |
| [setOnlyUseConnectionFile(boolean value)](#setOnlyUseConnectionFile-boolean-) | Indique si l'application de feuille de calcul doit toujours et uniquement utiliser les informations de connexion du fichier de connexion externe indiqué par l'attribut odcFile lors du rafraîchissement de la connexion. |
| [setParsePre(boolean value)](#setParsePre-boolean-) | Indicateur indiquant si les données contenues dans les balises HTML PRE de la page Web sont analysées en colonnes lors de l'importation de la page dans une table de requête. |
| [setPost(String value)](#setPost-java.lang.String-) | Renvoie ou définit la chaîne utilisée avec la méthode POST pour envoyer des données à un serveur Web afin de récupérer les données d'une requête Web. |
| [setReconnectionMethod(int value)](#setReconnectionMethod-int-) | Spécifie ce que l'application de feuille de calcul doit faire lorsqu'une connexion échoue. |
| [setReconnectionMethodType(int value)](#setReconnectionMethodType-int-) | Spécifie ce que l'application de feuille de calcul doit faire lorsqu'une connexion échoue. |
| [setRefreshInternal(int value)](#setRefreshInternal-int-) | Spécifie le nombre de minutes entre les rafraîchissements automatiques de la connexion. |
| [setRefreshOnLoad(boolean value)](#setRefreshOnLoad-boolean-) | Vrai si cette connexion doit être rafraîchie lors de l'ouverture du fichier ; sinon, faux. |
| [setSSOId(String value)](#setSSOId-java.lang.String-) | Identifiant pour l'authentification Single Sign On (SSO) utilisée entre un serveur intermédiaire spreadsheetML et la source de données externe. |
| [setSameSettings(boolean value)](#setSameSettings-boolean-) | Indicateur indiquant s'il faut analyser toutes les tables à l'intérieur d'un bloc PRE avec les mêmes paramètres de largeur que la première ligne. |
| [setSaveData(boolean value)](#setSaveData-boolean-) | Vrai si les données externes récupérées via la connexion pour remplir un tableau doivent être enregistrées avec le classeur ; sinon, faux. |
| [setSavePassword(boolean value)](#setSavePassword-boolean-) | Vrai si le mot de passe doit être enregistré dans la chaîne de connexion ; sinon, Faux. |
| [setSecondCommand(String value)](#setSecondCommand-java.lang.String-) | Spécifie une deuxième chaîne de texte de commande qui est conservée lorsque les champs de page basés sur le serveur PivotTable sont utilisés. |
| [setSourceFile(String value)](#setSourceFile-java.lang.String-) | Utilisé lorsque la source de données externe est basée sur un fichier. |
| [setSourceType(int value)](#setSourceType-int-) | Définit le type de DataSource de la connexion externe. |
| [setTextDates(boolean value)](#setTextDates-boolean-) | Indicateur indiquant si les dates doivent être importées dans les cellules de la feuille de calcul en tant que texte plutôt qu'en tant que dates. |
| [setType(int value)](#setType-int-) | Définit le type de DataSource de la connexion externe. |
| [setUrl(String value)](#setUrl-java.lang.String-) | URL à utiliser pour actualiser les données externes. |
| [setXl2000(boolean value)](#setXl2000-boolean-) | Ce drapeau existe pour assurer la compatibilité ascendante avec les anciens fichiers de feuille de calcul existants, et il est défini sur true si cette requête Web a été actualisée dans une application de feuille de calcul plus récente ou égale à Microsoft Excel 2000. |
| [setXl97(boolean value)](#setXl97-boolean-) | Ce drapeau existe pour assurer la compatibilité ascendante avec les anciens fichiers de feuille de calcul existants, et il est défini sur true si cette requête Web a été créée dans Microsoft Excel 97. |
| [setXml(boolean value)](#setXml-boolean-) | true si la source de la requête Web est XML (au lieu de HTML), sinon false. |
| [setXmlSourceData(boolean value)](#setXmlSourceData-boolean-) | Drapeau indiquant que les données source XML doivent être importées au lieu du tableau HTML lui‑même. |
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


Spécifie le type de commande OLE DB. 1. La requête indique un nom de cube 2. La requête indique une instruction SQL 3. La requête indique un nom de table 4. La requête indique que des informations par défaut ont été fournies, et il appartient au fournisseur de les interpréter. 5. La requête porte sur un fournisseur de données de liste basé sur le web.

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
### getEditPage() {#getEditPage--}
```
public String getEditPage()
```


L'URL de la page Web destinée à l'utilisateur affichant les données de la requête Web. Cette URL est conservée dans le cas où sourceData="true" et que l'url a été redirigée pour référencer un fichier XML. Ainsi, la page destinée à l'utilisateur peut être affichée dans l'interface, et les données XML peuvent être récupérées en arrière‑plan.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété WebQueryConnection.EditWebPage. Cette propriété sera supprimée 12 mois plus tard à compter d’octobre 2017. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
java.lang.String
### getEditWebPage() {#getEditWebPage--}
```
public String getEditWebPage()
```


L'URL de la page Web destinée à l'utilisateur affichant les données de la requête Web. Cette URL est conservée dans le cas où sourceData="true" et que l'url a été redirigée pour référencer un fichier XML. Ainsi, la page destinée à l'utilisateur peut être affichée dans l'interface, et les données XML peuvent être récupérées en arrière‑plan.

**Returns:**
java.lang.String
### getHtmlFormat() {#getHtmlFormat--}
```
public int getHtmlFormat()
```


Comment gérer le formatage provenant de la source HTML lors de l’importation des données de la requête Web dans la feuille de calcul. Pertinent lorsque sourceData est True.

Voir [HtmlFormatHandlingType](../../com.aspose.cells/htmlformathandlingtype).

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
### getPost() {#getPost--}
```
public String getPost()
```


Renvoie ou définit la chaîne utilisée avec la méthode POST pour envoyer des données à un serveur Web afin de récupérer les données d'une requête Web.

**Returns:**
java.lang.String
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
### getUrl() {#getUrl--}
```
public String getUrl()
```


URL à utiliser pour actualiser les données externes.

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isConsecutive() {#isConsecutive--}
```
public boolean isConsecutive()
```


Indicateur indiquant si les délimiteurs consécutifs doivent être traités comme un seul délimiteur.

**Returns:**
boolean
### isDeleted() {#isDeleted--}
```
public boolean isDeleted()
```


Indique si la connexion de classeur associée a été supprimée. true si la connexion a été supprimée ; sinon, false.

**Returns:**
boolean
### isHtmlTables() {#isHtmlTables--}
```
public boolean isHtmlTables()
```


Indicateur indiquant si les requêtes Web ne doivent fonctionner que sur les tableaux HTML.

**Returns:**
boolean
### isNew() {#isNew--}
```
public boolean isNew()
```


True si la connexion n’a pas été rafraîchie pour la première fois ; sinon, false. Cet état peut se produire lorsque l’utilisateur enregistre le fichier avant qu’une requête ne soit terminée.

**Returns:**
boolean
### isParsePre() {#isParsePre--}
```
public boolean isParsePre()
```


Indicateur indiquant si les données contenues dans les balises HTML PRE de la page Web sont analysées en colonnes lors de l'importation de la page dans une table de requête.

**Returns:**
boolean
### isSameSettings() {#isSameSettings--}
```
public boolean isSameSettings()
```


Indicateur indiquant s'il faut analyser toutes les tables à l'intérieur d'un bloc PRE avec les mêmes paramètres de largeur que la première ligne.

**Returns:**
boolean
### isTextDates() {#isTextDates--}
```
public boolean isTextDates()
```


Indicateur indiquant si les dates doivent être importées dans les cellules de la feuille de calcul en tant que texte plutôt qu'en tant que dates.

**Returns:**
boolean
### isXl2000() {#isXl2000--}
```
public boolean isXl2000()
```


Ce drapeau existe pour assurer la compatibilité ascendante avec les anciens fichiers de feuille de calcul existants, et il est défini sur true si cette requête Web a été actualisée dans une application de feuille de calcul plus récente ou égale à Microsoft Excel 2000. C’est un attribut optionnel qui peut être ignoré.

**Returns:**
boolean
### isXl97() {#isXl97--}
```
public boolean isXl97()
```


Ce drapeau existe pour assurer la compatibilité ascendante avec les anciens fichiers de feuille de calcul existants, et il est défini sur true si cette requête Web a été créée dans Microsoft Excel 97. C’est un attribut optionnel qui peut être ignoré.

**Returns:**
boolean
### isXml() {#isXml--}
```
public boolean isXml()
```


true si la source de la requête Web est XML (au lieu de HTML), sinon false.

**Returns:**
boolean
### isXmlSourceData() {#isXmlSourceData--}
```
public boolean isXmlSourceData()
```


Drapeau indiquant que les données source XML doivent être importées au lieu du tableau HTML lui‑même.

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


Spécifie le type de commande OLE DB. 1. La requête indique un nom de cube 2. La requête indique une instruction SQL 3. La requête indique un nom de table 4. La requête indique que des informations par défaut ont été fournies, et il appartient au fournisseur de les interpréter. 5. La requête porte sur un fournisseur de données de liste basé sur le web.

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

### setConsecutive(boolean value) {#setConsecutive-boolean-}
```
public void setConsecutive(boolean value)
```


Indicateur indiquant si les délimiteurs consécutifs doivent être traités comme un seul délimiteur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

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

### setEditPage(String value) {#setEditPage-java.lang.String-}
```
public void setEditPage(String value)
```


L'URL de la page Web destinée à l'utilisateur affichant les données de la requête Web. Cette URL est conservée dans le cas où sourceData="true" et que l'url a été redirigée pour référencer un fichier XML. Ainsi, la page destinée à l'utilisateur peut être affichée dans l'interface, et les données XML peuvent être récupérées en arrière‑plan.

**Remarks**

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété WebQueryConnection.EditWebPage. Cette propriété sera supprimée 12 mois plus tard à compter d’octobre 2017. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setEditWebPage(String value) {#setEditWebPage-java.lang.String-}
```
public void setEditWebPage(String value)
```


L'URL de la page Web destinée à l'utilisateur affichant les données de la requête Web. Cette URL est conservée dans le cas où sourceData="true" et que l'url a été redirigée pour référencer un fichier XML. Ainsi, la page destinée à l'utilisateur peut être affichée dans l'interface, et les données XML peuvent être récupérées en arrière‑plan.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setHtmlFormat(int value) {#setHtmlFormat-int-}
```
public void setHtmlFormat(int value)
```


Comment gérer le formatage provenant de la source HTML lors de l’importation des données de la requête Web dans la feuille de calcul. Pertinent lorsque sourceData est True.

Voir [HtmlFormatHandlingType](../../com.aspose.cells/htmlformathandlingtype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setHtmlTables(boolean value) {#setHtmlTables-boolean-}
```
public void setHtmlTables(boolean value)
```


Indicateur indiquant si les requêtes Web ne doivent fonctionner que sur les tableaux HTML.

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

### setParsePre(boolean value) {#setParsePre-boolean-}
```
public void setParsePre(boolean value)
```


Indicateur indiquant si les données contenues dans les balises HTML PRE de la page Web sont analysées en colonnes lors de l'importation de la page dans une table de requête.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setPost(String value) {#setPost-java.lang.String-}
```
public void setPost(String value)
```


Renvoie ou définit la chaîne utilisée avec la méthode POST pour envoyer des données à un serveur Web afin de récupérer les données d'une requête Web.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

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

### setSameSettings(boolean value) {#setSameSettings-boolean-}
```
public void setSameSettings(boolean value)
```


Indicateur indiquant s'il faut analyser toutes les tables à l'intérieur d'un bloc PRE avec les mêmes paramètres de largeur que la première ligne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

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

### setTextDates(boolean value) {#setTextDates-boolean-}
```
public void setTextDates(boolean value)
```


Indicateur indiquant si les dates doivent être importées dans les cellules de la feuille de calcul en tant que texte plutôt qu'en tant que dates.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

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

### setUrl(String value) {#setUrl-java.lang.String-}
```
public void setUrl(String value)
```


URL à utiliser pour actualiser les données externes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setXl2000(boolean value) {#setXl2000-boolean-}
```
public void setXl2000(boolean value)
```


Ce drapeau existe pour assurer la compatibilité ascendante avec les anciens fichiers de feuille de calcul existants, et il est défini sur true si cette requête Web a été actualisée dans une application de feuille de calcul plus récente ou égale à Microsoft Excel 2000. C’est un attribut optionnel qui peut être ignoré.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setXl97(boolean value) {#setXl97-boolean-}
```
public void setXl97(boolean value)
```


Ce drapeau existe pour assurer la compatibilité ascendante avec les anciens fichiers de feuille de calcul existants, et il est défini sur true si cette requête Web a été créée dans Microsoft Excel 97. C’est un attribut optionnel qui peut être ignoré.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setXml(boolean value) {#setXml-boolean-}
```
public void setXml(boolean value)
```


true si la source de la requête Web est XML (au lieu de HTML), sinon false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setXmlSourceData(boolean value) {#setXmlSourceData-boolean-}
```
public void setXmlSourceData(boolean value)
```


Drapeau indiquant que les données source XML doivent être importées au lieu du tableau HTML lui‑même.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

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

