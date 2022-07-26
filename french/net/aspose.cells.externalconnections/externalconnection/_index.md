---
title: ExternalConnection
second_title: Référence de l'API Aspose.Cells pour .NET
description: Spécifie une connexion de données externe
type: docs
weight: 3290
url: /fr/net/aspose.cells.externalconnections/externalconnection/
---
## ExternalConnection class

Spécifie une connexion de données externe

```csharp
public abstract class ExternalConnection
```

## Propriétés

| Nom | La description |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh) { get; set; } | Indique si la connexion peut être actualisée en arrière-plan (de manière asynchrone). true si l'utilisation préférée de la connexion consiste à actualiser de manière asynchrone en arrière-plan ; false si l'utilisation préférée de la connexion consiste à actualiser de manière synchrone au premier plan. |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription) { get; set; } | Spécifie la description de l'utilisateur pour cette connexion |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid) { get; } | Spécifie l'identifiant unique de cette connexion. |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype) { get; set; } | Spécifie la méthode d'authentification à utiliser lors de l'établissement (ou du rétablissement) de la connexion. |
| [Id](../../aspose.cells.externalconnections/externalconnection/id) { get; } | Obtient l'identifiant de la connexion. |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted) { get; set; } | Indique si la connexion au classeur associé a été supprimée. true si la connexion the a été supprimée ; sinon, faux. |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew) { get; set; } | Vrai si la connexion n'a pas été actualisée pour la première fois ; sinon, faux. Cet état peut se produire lorsque l'utilisateur enregistre le fichier avant qu'une requête n'ait fini de renvoyer. |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive) { get; set; } | Vrai lorsque le tableur doit s'efforcer de maintenir la connexion ouverte. Si false, l'application doit fermer la connexion après avoir récupéré les informations . |
| [Name](../../aspose.cells.externalconnections/externalconnection/name) { get; set; } | Spécifie le nom de la connexion. Chaque connexion doit avoir un nom unique. |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile) { get; set; } | Spécifie le chemin d'accès complet au fichier de connexion externe à partir duquel cette connexion a été créée. Si une connexion échoue lors d'une tentative d'actualisation des données et que reconnectionMethod=1, , l'application de feuille de calcul réessaye en utilisant les informations du fichier de connexion externe au lieu de l'objet de connexion intégré dans le classeur. |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile) { get; set; } | Indique si le tableur doit toujours et uniquement utiliser les informations de connexion dans le fichier de connexion externe indiqué par l'attribut odcFile lorsque la connexion est actualisée. Si false, l'application de feuille de calcul doit suivre la procédure indiquée par l'attribut reconnectionMethod |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters) { get; } | Obtient[`ConnectionParameterCollection`](../connectionparametercollection) pour une requête ODBC ou Web. |
| virtual [PowerQueryFormula](../../aspose.cells.externalconnections/externalconnection/powerqueryformula) { get; } | Obtient la définition de la formule de requête de puissance. |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype) { get; set; } | Spécifie ce que l'application de feuille de calcul doit faire lorsqu'une connexion échoue. La valeur par défaut est ReConnectionMethodType.Required. |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal) { get; set; } | Spécifie le nombre de minutes entre les actualisations automatiques de la connexion. |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload) { get; set; } | Vrai si cette connexion doit être rafraichie à l'ouverture du fichier ; sinon, faux. |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata) { get; set; } | True si les données externes extraites via la connexion pour remplir une table doivent être enregistrées avec le classeur ; sinon, faux. |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword) { get; set; } | Vrai si le mot de passe doit être enregistré dans le cadre de la chaîne de connexion ; sinon, Faux. |
| [SourceFile](../../aspose.cells.externalconnections/externalconnection/sourcefile) { get; set; } | Utilisé lorsque la source de données externe est basée sur un fichier. Lorsqu'une connexion à une telle source de données échoue, le tableur tente de se connecter directement à ce fichier. Peut être exprimé en URI ou en notation de chemin de fichier spécifique au système. |
| [SSOId](../../aspose.cells.externalconnections/externalconnection/ssoid) { get; set; } | Identifiant pour l'authentification unique (SSO) utilisé pour l'authentification entre un serveur spreadsheetML intermédiaire et la source de données externe. |
| [Type](../../aspose.cells.externalconnections/externalconnection/type) { get; set; } | Obtient ou définit le type de source de données de la connexion externe. |

### Voir également

* espace de noms [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
