---
title: "WebQueryConnection Classe"
linktitle: "WebQueryConnection"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "WebQueryConnection classe. Encapsule l'objet qui représente webqueryconnection en Go."
type: docs
weight: 200
url: /fr/go-cpp/webqueryconnection/
---

## WebQueryConnection class

Spécifie les propriétés d'une source de requête Web. Une requête Web récupère les données des tables HTML et peut également fournir des paramètres HTTP "Get" à traiter par le serveur Web lors de la génération du HTML en incluant les paramètres et les éléments de paramètres.

```go

type WebQueryConnection struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewWebQueryConnection](./newwebqueryconnection/) | Construit à partir d'un objet parent. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetClassType](./getclasstype/) | Obtient le type de cet objet ExternalConnection. |
| [IsXml](./isxml/) | true si la source de la requête web est XML (par opposition à HTML), sinon false. |
| [SetIsXml](./setisxml/) | true si la source de la requête web est XML (par opposition à HTML), sinon false. |
| [IsXl97](./isxl97/) | Ce drapeau existe pour la compatibilité ascendante avec d'anciennes feuilles de calcul existantes, et est défini sur true si cette requête web a été créée dans Microsoft Excel 97.Ceci est un attribut optionnel qui peut être ignoré. |
| [SetIsXl97](./setisxl97/) | Ce drapeau existe pour la compatibilité ascendante avec d'anciennes feuilles de calcul existantes, et est défini sur true si cette requête web a été créée dans Microsoft Excel 97.Ceci est un attribut optionnel qui peut être ignoré. |
| [IsXl2000](./isxl2000/) | Ce drapeau existe pour la compatibilité ascendante avec d'anciennes feuilles de calcul existantes, et est défini sur true si cette requête web a été actualisée dans une application de feuille de calcul plus récente ou égale à Microsoft Excel 2000.Ceci est un attribut optionnel qui peut être ignoré. |
| [SetIsXl2000](./setisxl2000/) | Ce drapeau existe pour la compatibilité ascendante avec d'anciennes feuilles de calcul existantes, et est défini sur true si cette requête web a été actualisée dans une application de feuille de calcul plus récente ou égale à Microsoft Excel 2000.Ceci est un attribut optionnel qui peut être ignoré. |
| [GetUrl](./geturl/) | URL à utiliser pour actualiser les données externes. |
| [SetUrl](./seturl/) | URL à utiliser pour actualiser les données externes. |
| [GetConnectionFile](./getconnectionfile/) | Obtient le fichier de connexion. |
| [IsTextDates](./istextdates/) | Drapeau indiquant si les dates doivent être importées dans les cellules de la feuille de calcul en tant que texte plutôt qu'en tant que dates. |
| [SetIsTextDates](./setistextdates/) | Drapeau indiquant si les dates doivent être importées dans les cellules de la feuille de calcul en tant que texte plutôt qu'en tant que dates. |
| [IsXmlSourceData](./isxmlsourcedata/) | Drapeau indiquant que les données source XML doivent être importées à la place du tableau HTML lui‑même. |
| [SetIsXmlSourceData](./setisxmlsourcedata/) | Drapeau indiquant que les données source XML doivent être importées à la place du tableau HTML lui‑même. |
| [GetPost](./getpost/) | Renvoie ou définit la chaîne utilisée avec la méthode POST pour saisir des données dans un serveur web afin de renvoyer des données d'une requête web. |
| [SetPost](./setpost/) | Renvoie ou définit la chaîne utilisée avec la méthode POST pour saisir des données dans un serveur web afin de renvoyer des données d'une requête web. |
| [IsParsePre](./isparsepre/) | Drapeau indiquant si les données contenues dans les balises HTML PRE de la page web sont analysées en colonnes lorsque vous importez la page dans une table de requête. |
| [SetIsParsePre](./setisparsepre/) | Drapeau indiquant si les données contenues dans les balises HTML PRE de la page web sont analysées en colonnes lorsque vous importez la page dans une table de requête. |
| [IsHtmlTables](./ishtmltables/) | Drapeau indiquant si les requêtes web ne doivent fonctionner que sur des tableaux HTML. |
| [SetIsHtmlTables](./setishtmltables/) | Drapeau indiquant si les requêtes web ne doivent fonctionner que sur des tableaux HTML. |
| [GetHtmlFormat](./gethtmlformat/) | Comment gérer le formatage provenant de la source HTML lors de l'importation des données de requête web dans la feuille de calcul. Pertinent lorsque sourceData est True. |
| [SetHtmlFormat](./sethtmlformat/) | Comment gérer le formatage provenant de la source HTML lors de l'importation des données de requête web dans la feuille de calcul. Pertinent lorsque sourceData est True. |
| [IsSameSettings](./issamesettings/) | Drapeau indiquant s'il faut analyser toutes les tables à l'intérieur d'un bloc PRE avec les mêmes paramètres de largeur que la première ligne. |
| [SetIsSameSettings](./setissamesettings/) | Drapeau indiquant s'il faut analyser toutes les tables à l'intérieur d'un bloc PRE avec les mêmes paramètres de largeur que la première ligne. |
| [GetEditWebPage](./geteditwebpage/) | L'URL de la page web destinée à l'utilisateur affichant les données de la requête web. Cette URL est conservée dans le cas où sourceData=\"true\" et que l'url a été redirigée pour référencer un fichier XML.Alors la page destinée à l'utilisateur peut être affichée dans l'interface utilisateur, et les données XML peuvent être récupérées en arrière‑plan. |
| [SetEditWebPage](./seteditwebpage/) | L'URL de la page web destinée à l'utilisateur affichant les données de la requête web. Cette URL est conservée dans le cas où sourceData=\"true\" et que l'url a été redirigée pour référencer un fichier XML.Alors la page destinée à l'utilisateur peut être affichée dans l'interface utilisateur, et les données XML peuvent être récupérées en arrière‑plan. |
| [IsConsecutive](./isconsecutive/) | Drapeau indiquant si les délimiteurs consécutifs doivent être traités comme un seul délimiteur. |
| [SetIsConsecutive](./setisconsecutive/) | Drapeau indiquant si les délimiteurs consécutifs doivent être traités comme un seul délimiteur. |
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
| [GetCommand](./getcommand/) | La chaîne contenant la commande de base de données à transmettre à l'API du fournisseur de données qui interagira avec la source externe afin de récupérer les données |
| [SetCommand](./setcommand/) | La chaîne contenant la commande de base de données à transmettre à l'API du fournisseur de données qui interagira avec la source externe afin de récupérer les données |
| [GetCommandType](./getcommandtype/) | Spécifie le type de commande OLE DB. 1. La requête spécifie un nom de cube 2. La requête spécifie une instruction SQL 3. La requête spécifie un nom de table 4. La requête indique que des informations par défaut ont été fournies, et il appartient au fournisseur de les interpréter. 5. La requête porte sur un fournisseur de données de liste basé sur le web. |
| [SetCommandType](./setcommandtype/) | Spécifie le type de commande OLE DB. 1. La requête spécifie un nom de cube 2. La requête spécifie une instruction SQL 3. La requête spécifie un nom de table 4. La requête indique que des informations par défaut ont été fournies, et il appartient au fournisseur de les interpréter. 5. La requête porte sur un fournisseur de données de liste basé sur le web. |
| [GetConnectionString](./getconnectionstring/) | La chaîne d'informations de connexion est utilisée pour établir le contact avec une source de données OLE DB ou ODBC. |
| [SetConnectionString](./setconnectionstring/) | La chaîne d'informations de connexion est utilisée pour établir le contact avec une source de données OLE DB ou ODBC. |
| [GetSecondCommand](./getsecondcommand/) | Spécifie une deuxième chaîne de texte de commande qui est conservée lorsque les champs de page basés sur le serveur de PivotTable sont utilisés. Pour les connexions ODBC, serverCommand est généralement une requête plus large que command (aucune clause WHERE n'est présente dans la première). En se basant sur ces 2 commandes (Command et ServerCommand), l'interface utilisateur des paramètres peut être remplie et des requêtes paramétrées peuvent être construites. |
| [SetSecondCommand](./setsecondcommand/) | Spécifie une deuxième chaîne de texte de commande qui est conservée lorsque les champs de page basés sur le serveur de PivotTable sont utilisés. Pour les connexions ODBC, serverCommand est généralement une requête plus large que command (aucune clause WHERE n'est présente dans la première). En se basant sur ces 2 commandes (Command et ServerCommand), l'interface utilisateur des paramètres peut être remplie et des requêtes paramétrées peuvent être construites. |
