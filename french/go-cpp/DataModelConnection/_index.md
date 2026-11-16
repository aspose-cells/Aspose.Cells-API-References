---
title: "DataModelConnection Classe"
linktitle: "DataModelConnection"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "DataModelConnection class. Encapsule l'objet qui représente datamodelconnection en Go."
type: docs
weight: 200
url: /fr/go-cpp/datamodelconnection/
---

## DataModelConnection class

Spécifie une connexion de modèle de données

```go

type DataModelConnection struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewDataModelConnection](./newdatamodelconnection/) | Construit à partir d'un objet parent. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetClassType](./getclasstype/) | Obtient le type de cet objet ExternalConnection. |
| [GetCommand](./getcommand/) | La chaîne contenant la commande de base de données à transmettre à l'API du fournisseur de données qui interagira avec la source externe afin de récupérer les données |
| [SetCommand](./setcommand/) | La chaîne contenant la commande de base de données à transmettre à l'API du fournisseur de données qui interagira avec la source externe afin de récupérer les données |
| [GetCommandType](./getcommandtype/) | Renvoie le type OLEDBCommandType. |
| [SetCommandType](./setcommandtype/) | Renvoie le type OLEDBCommandType. |
| [GetConnectionString](./getconnectionstring/) | La chaîne d'informations de connexion est utilisée pour établir le contact avec une source de données OLE DB ou ODBC. |
| [SetConnectionString](./setconnectionstring/) | La chaîne d'informations de connexion est utilisée pour établir le contact avec une source de données OLE DB ou ODBC. |
| [GetId](./getid/) | Obtient l'identifiant de la connexion. |
| [GetSourceType](./getsourcetype/) | Obtient ou définit le type DataSource de la connexion externe. |
| [SetSourceType](./setsourcetype/) | Obtient ou définit le type DataSource de la connexion externe. |
| [GetSSOId](./getssoid/) | Identifiant pour Single Sign On (SSO) utilisé pour l'authentification entre un serveur intermédiaire spreadsheetML et la source de données externe. |
| [SetSSOId](./setssoid/) | Identifiant pour Single Sign On (SSO) utilisé pour l'authentification entre un serveur intermédiaire spreadsheetML et la source de données externe. |
| [GetSavePassword](./getsavepassword/) | Vrai si le mot de passe doit être enregistré dans la chaîne de connexion ; sinon, Faux. |
| [SetSavePassword](./setsavepassword/) | Vrai si le mot de passe doit être enregistré dans la chaîne de connexion ; sinon, Faux. |
| [GetSaveData](./getsavedata/) | Vrai si les données externes récupérées via la connexion pour remplir une table doivent être enregistrées avec le classeur ; sinon, faux. |
| [SetSaveData](./setsavedata/) | Vrai si les données externes récupérées via la connexion pour remplir une table doivent être enregistrées avec le classeur ; sinon, faux. |
| [GetRefreshOnLoad](./getrefreshonload/) | Vrai si cette connexion doit être actualisée lors de l'ouverture du fichier ; sinon, faux. |
| [SetRefreshOnLoad](./setrefreshonload/) | Vrai si cette connexion doit être actualisée lors de l'ouverture du fichier ; sinon, faux. |
| [GetReconnectionMethodType](./getreconnectionmethodtype/) | Spécifie ce que l'application de feuille de calcul doit faire lorsqu'une connexion échoue. La valeur par défaut est ReConnectionMethodType.Required. |
| [SetReconnectionMethodType](./setreconnectionmethodtype/) | Spécifie ce que l'application de feuille de calcul doit faire lorsqu'une connexion échoue. La valeur par défaut est ReConnectionMethodType.Required. |
| [GetOnlyUseConnectionFile](./getonlyuseconnectionfile/) | Indique si l'application de feuille de calcul doit toujours et uniquement utiliser les informations de connexion du fichier de connexion externe indiqué par l'attribut odcFile lors du rafraîchissement de la connexion. Si faux, alors l'application de feuille de calcul doit suivre la procédure indiquée par l'attribut reconnectionMethod. |
| [SetOnlyUseConnectionFile](./setonlyuseconnectionfile/) | Indique si l'application de feuille de calcul doit toujours et uniquement utiliser les informations de connexion du fichier de connexion externe indiqué par l'attribut odcFile lors du rafraîchissement de la connexion. Si faux, alors l'application de feuille de calcul doit suivre la procédure indiquée par l'attribut reconnectionMethod. |
| [GetOdcFile](./getodcfile/) | Spécifie le chemin complet vers le fichier de connexion externe à partir duquel cette connexion a été créée. Si une connexion échoue lors d'une tentative d'actualisation des données, et reconnectionMethod=1, l'application de feuille de calcul réessaiera en utilisant les informations du fichier de connexion externe au lieu de l'objet de connexion intégré au classeur. |
| [SetOdcFile](./setodcfile/) | Spécifie le chemin complet vers le fichier de connexion externe à partir duquel cette connexion a été créée. Si une connexion échoue lors d'une tentative d'actualisation des données, et reconnectionMethod=1, l'application de feuille de calcul réessaiera en utilisant les informations du fichier de connexion externe au lieu de l'objet de connexion intégré au classeur. |
| [GetSourceFile](./getsourcefile/) | Utilisé lorsque la source de données externe est basée sur un fichier. Lorsqu'une connexion à une telle source échoue, l'application de feuille de calcul tente de se connecter directement à ce fichier. Peut être exprimé en URI ou en notation de chemin de fichier spécifique au système. |
| [SetSourceFile](./setsourcefile/) | Utilisé lorsque la source de données externe est basée sur un fichier. Lorsqu'une connexion à une telle source échoue, l'application de feuille de calcul tente de se connecter directement à ce fichier. Peut être exprimé en URI ou en notation de chemin de fichier spécifique au système. |
| [IsNew](./isnew/) | Vrai si la connexion n'a pas été actualisée pour la première fois ; sinon, faux. Cet état peut se produire lorsque l'utilisateur enregistre le fichier avant que la requête ne soit terminée. |
| [SetIsNew](./setisnew/) | Vrai si la connexion n'a pas été actualisée pour la première fois ; sinon, faux. Cet état peut se produire lorsque l'utilisateur enregistre le fichier avant que la requête ne soit terminée. |
| [GetName](./getname/) | Spécifie le nom de la connexion. Chaque connexion doit avoir un nom unique. |
| [SetName](./setname/) | Spécifie le nom de la connexion. Chaque connexion doit avoir un nom unique. |
| [GetKeepAlive](./getkeepalive/) | Vrai lorsque l'application de feuille de calcul doit faire des efforts pour maintenir la connexion ouverte. Si faux, l'application doit fermer la connexion après avoir récupéré l'information. |
| [SetKeepAlive](./setkeepalive/) | Vrai lorsque l'application de feuille de calcul doit faire des efforts pour maintenir la connexion ouverte. Si faux, l'application doit fermer la connexion après avoir récupéré l'information. |
| [GetRefreshInternal](./getrefreshinternal/) | Spécifie le nombre de minutes entre les actualisations automatiques de la connexion. |
| [SetRefreshInternal](./setrefreshinternal/) | Spécifie le nombre de minutes entre les actualisations automatiques de la connexion. |
| [GetConnectionDescription](./getconnectiondescription/) | Spécifie la description utilisateur pour cette connexion |
| [SetConnectionDescription](./setconnectiondescription/) | Spécifie la description utilisateur pour cette connexion |
| [IsDeleted](./isdeleted/) | Indique si la connexion du classeur associée a été supprimée. vrai si la connexion a été supprimée ; sinon, faux. |
| [SetIsDeleted](./setisdeleted/) | Indique si la connexion du classeur associée a été supprimée. vrai si la connexion a été supprimée ; sinon, faux. |
| [GetCredentialsMethodType](./getcredentialsmethodtype/) | Spécifie la méthode d'authentification à utiliser lors de l'établissement (ou du rétablissement) de la connexion. |
| [SetCredentialsMethodType](./setcredentialsmethodtype/) | Spécifie la méthode d'authentification à utiliser lors de l'établissement (ou du rétablissement) de la connexion. |
| [GetBackgroundRefresh](./getbackgroundrefresh/) | Indique si la connexion peut être actualisée en arrière-plan (asynchroniquement). vrai si l'utilisation préférée de la connexion est de rafraîchir de façon asynchrone en arrière-plan ; faux si l'utilisation préférée de la connexion est de rafraîchir de façon synchrone au premier plan. |
| [SetBackgroundRefresh](./setbackgroundrefresh/) | Indique si la connexion peut être actualisée en arrière-plan (asynchroniquement). vrai si l'utilisation préférée de la connexion est de rafraîchir de façon asynchrone en arrière-plan ; faux si l'utilisation préférée de la connexion est de rafraîchir de façon synchrone au premier plan. |
| [GetParameters](./getparameters/) | Obtient ConnectionParameterCollection pour une requête ODBC ou web. |
| [GetPowerQueryFormula](./getpowerqueryformula/) | Obtient la définition de la formule Power Query. |
| [GetConnectionFile](./getconnectionfile/) | Obtient le fichier de connexion. |
| [GetSecondCommand](./getsecondcommand/) | Spécifie une deuxième chaîne de texte de commande qui est conservée lorsque les champs de page basés sur le serveur de PivotTable sont utilisés. Pour les connexions ODBC, serverCommand est généralement une requête plus large que command (aucune clause WHERE n'est présente dans la première). En se basant sur ces 2 commandes (Command et ServerCommand), l'interface utilisateur des paramètres peut être remplie et des requêtes paramétrées peuvent être construites. |
| [SetSecondCommand](./setsecondcommand/) | Spécifie une deuxième chaîne de texte de commande qui est conservée lorsque les champs de page basés sur le serveur de PivotTable sont utilisés. Pour les connexions ODBC, serverCommand est généralement une requête plus large que command (aucune clause WHERE n'est présente dans la première). En se basant sur ces 2 commandes (Command et ServerCommand), l'interface utilisateur des paramètres peut être remplie et des requêtes paramétrées peuvent être construites. |
