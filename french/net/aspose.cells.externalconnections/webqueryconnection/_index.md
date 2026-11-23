---
title: "Classe WebQueryConnection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.ExternalConnections.WebQueryConnection. Spécifie les propriétés d'une source de requête Web. Une requête Web récupérera des données à partir de tables HTML et peut également fournir des paramètres HTTP GET à traiter par le serveur Web lors de la génération du HTML en incluant les paramètres et les éléments de paramètre."
type: docs
url: /fr/net/aspose.cells.externalconnections/webqueryconnection/
---
## WebQueryConnection class

Spécifie les propriétés d'une source de requête Web. Une requête Web récupérera des données à partir de tables HTML, et peut également fournir des paramètres HTTP "Get" à traiter par le serveur Web lors de la génération du HTML en incluant les paramètres et les éléments de paramètres.

```csharp
public class WebQueryConnection : ExternalConnection
```

## Propriétés

| Nom | Description |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh/) { get; set; } | Indique si la connexion peut être rafraîchie en arrière-plan (asynchroniquement). true si l’utilisation préférée de la connexion est de rafraîchir de façon asynchrone en arrière-plan ; false si l’utilisation préférée de la connexion est de rafraîchir de façon synchrone au premier plan.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| override [ClassType](../../aspose.cells.externalconnections/webqueryconnection/classtype/) { get; } | Obtient le type de cet objet [`ExternalConnection`](../externalconnection/). |
| virtual [Command](../../aspose.cells.externalconnections/externalconnection/command/) { get; set; } | La chaîne contenant la commande de base de données à transmettre à l'API du fournisseur de données qui interagira avec la source externe afin de récupérer les données (Héritée de [`ExternalConnection`](../externalconnection/).) |
| virtual [CommandType](../../aspose.cells.externalconnections/externalconnection/commandtype/) { get; set; } | Spécifie le type de commande OLE DB. 1. La requête spécifie un nom de cube 2. La requête spécifie une instruction SQL 3. La requête spécifie un nom de table 4. La requête indique que des informations par défaut ont été données, et il revient au fournisseur de les interpréter. 5. La requête s'adresse à un fournisseur de données de liste basé sur le Web. (Héritée de [`ExternalConnection`](../externalconnection/).) |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription/) { get; set; } | Spécifie la description utilisateur pour cette connexion(Inherited from [`ExternalConnection`](../externalconnection/).) |
| override [ConnectionFile](../../aspose.cells.externalconnections/webqueryconnection/connectionfile/) { get; } | Obtient le fichier de connexion. |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid/) { get; } | (**Obsolete.**) Spécifie l’identifiant unique de cette connexion.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| virtual [ConnectionString](../../aspose.cells.externalconnections/externalconnection/connectionstring/) { get; set; } | La chaîne d'informations de connexion est utilisée pour établir le contact avec une source de données OLE DB ou ODBC. (Héritée de [`ExternalConnection`](../externalconnection/).) |
| [Credentials](../../aspose.cells.externalconnections/externalconnection/credentials/) { get; set; } | (**Obsolete.**) Spécifie la méthode d’authentification à utiliser lors de l’établissement (ou du ré‑établissement) de la connexion.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype/) { get; set; } | Spécifie la méthode d’authentification à utiliser lors de l’établissement (ou du ré‑établissement) de la connexion.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [EditPage](../../aspose.cells.externalconnections/webqueryconnection/editpage/) { get; set; } | (**Obsolete.**) L'URL de la page Web destinée à l'utilisateur affichant les données de la requête Web. Cette URL est conservée dans le cas où sourceData="true" et que l'url a été redirigée pour référencer un fichier XML. Ainsi, la page destinée à l'utilisateur peut être affichée dans l'interface, et les données XML peuvent être récupérées en arrière-plan. |
| [EditWebPage](../../aspose.cells.externalconnections/webqueryconnection/editwebpage/) { get; set; } | L'URL de la page Web destinée à l'utilisateur affichant les données de la requête Web. Cette URL est conservée dans le cas où sourceData="true" et que l'url a été redirigée pour référencer un fichier XML. Ainsi, la page destinée à l'utilisateur peut être affichée dans l'interface, et les données XML peuvent être récupérées en arrière-plan. |
| [HtmlFormat](../../aspose.cells.externalconnections/webqueryconnection/htmlformat/) { get; set; } | Comment gérer le formatage provenant de la source HTML lors de l'importation des données de requête Web dans la feuille de calcul. Pertinent lorsque sourceData est True. |
| [Id](../../aspose.cells.externalconnections/externalconnection/id/) { get; } | Obtient l’identifiant de la connexion.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [IsConsecutive](../../aspose.cells.externalconnections/webqueryconnection/isconsecutive/) { get; set; } | Indicateur indiquant si les délimiteurs consécutifs doivent être traités comme un seul délimiteur. |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted/) { get; set; } | Indique si la connexion de classeur associée a été supprimée. true si la connexion a été supprimée ; sinon, false.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [IsHtmlTables](../../aspose.cells.externalconnections/webqueryconnection/ishtmltables/) { get; set; } | Indicateur indiquant si les requêtes Web ne doivent fonctionner que sur des tables HTML. |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew/) { get; set; } | True si la connexion n’a pas été rafraîchie pour la première fois ; sinon, false. Cet état peut se produire lorsque l’utilisateur enregistre le fichier avant qu’une requête ne soit terminée.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [IsParsePre](../../aspose.cells.externalconnections/webqueryconnection/isparsepre/) { get; set; } | Indicateur indiquant si les données contenues dans les balises HTML PRE de la page Web sont analysées en colonnes lors de l'importation de la page dans une table de requête. |
| [IsSameSettings](../../aspose.cells.externalconnections/webqueryconnection/issamesettings/) { get; set; } | Indicateur indiquant s'il faut analyser toutes les tables à l'intérieur d'un bloc PRE avec les mêmes paramètres de largeur que la première ligne. |
| [IsTextDates](../../aspose.cells.externalconnections/webqueryconnection/istextdates/) { get; set; } | Indicateur indiquant si les dates doivent être importées dans les cellules de la feuille de calcul en tant que texte plutôt qu'en tant que dates. |
| [IsXl2000](../../aspose.cells.externalconnections/webqueryconnection/isxl2000/) { get; set; } | Ce drapeau existe pour assurer la compatibilité descendante avec d'anciens fichiers de feuille de calcul, et il est réglé sur true si cette requête Web a été actualisée dans une application de feuille de calcul plus récente ou égale à Microsoft Excel 2000. C'est un attribut optionnel qui peut être ignoré. |
| [IsXl97](../../aspose.cells.externalconnections/webqueryconnection/isxl97/) { get; set; } | Ce drapeau existe pour assurer la compatibilité descendante avec d'anciens fichiers de feuille de calcul, et il est réglé sur true si cette requête Web a été créée dans Microsoft Excel 97. C'est un attribut optionnel qui peut être ignoré. |
| [IsXml](../../aspose.cells.externalconnections/webqueryconnection/isxml/) { get; set; } | true si la source de la requête Web est XML (par opposition à HTML), sinon false. |
| [IsXmlSourceData](../../aspose.cells.externalconnections/webqueryconnection/isxmlsourcedata/) { get; set; } | Drapeau indiquant que les données source XML doivent être importées au lieu du tableau HTML lui‑même. |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive/) { get; set; } | True lorsque l’application de feuille de calcul doit s’efforcer de garder la connexion ouverte. false lorsque l’application doit fermer la connexion après avoir récupéré les informations.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [Name](../../aspose.cells.externalconnections/externalconnection/name/) { get; set; } | Spécifie le nom de la connexion. Chaque connexion doit avoir un nom unique.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile/) { get; set; } | Spécifie le chemin complet du fichier de connexion externe à partir duquel cette connexion a été créée. Si une connexion échoue lors d’une tentative de rafraîchissement des données, et reconnectionMethod=1, alors l’application de feuille de calcul réessaiera en utilisant les informations du fichier de connexion externe au lieu de l’objet de connexion intégré dans le classeur.(Hérité de [`ExternalConnection`](../externalconnection/).) |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile/) { get; set; } | Indique si l’application de feuille de calcul doit toujours et uniquement utiliser les informations de connexion du fichier de connexion externe indiqué par l’attribut odcFile lors du rafraîchissement de la connexion. Si false, alors l’application de feuille de calcul doit suivre la procédure indiquée par l’attribut reconnectionMethod.(Hérité de [`ExternalConnection`](../externalconnection/).) |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters/) { get; } | Obtient [`ConnectionParameterCollection`](../connectionparametercollection/) pour une requête ODBC ou Web.(Hérité de [`ExternalConnection`](../externalconnection/).) |
| [Post](../../aspose.cells.externalconnections/webqueryconnection/post/) { get; set; } | Renvoie ou définit la chaîne utilisée avec la méthode post pour envoyer des données à un serveur Web afin de récupérer les données d’une requête Web. |
| virtual [PowerQueryFormula](../../aspose.cells.externalconnections/externalconnection/powerqueryformula/) { get; } | Obtient la définition de la formule Power Query.(Hérité de [`ExternalConnection`](../externalconnection/).) |
| [ReconnectionMethod](../../aspose.cells.externalconnections/externalconnection/reconnectionmethod/) { get; set; } | (**Obsolete.**) Spécifie ce que l’application de feuille de calcul doit faire lorsqu’une connexion échoue. La valeur par défaut est ReConnectionMethodType.Required.(Hérité de [`ExternalConnection`](../externalconnection/).) |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype/) { get; set; } | Spécifie ce que l’application de feuille de calcul doit faire lorsqu’une connexion échoue. La valeur par défaut est ReConnectionMethodType.Required.(Hérité de [`ExternalConnection`](../externalconnection/).) |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal/) { get; set; } | Spécifie le nombre de minutes entre les rafraîchissements automatiques de la connexion.(Hérité de [`ExternalConnection`](../externalconnection/).) |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload/) { get; set; } | True si cette connexion doit être rafraîchie à l’ouverture du fichier ; sinon, false.(Hérité de [`ExternalConnection`](../externalconnection/).) |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata/) { get; set; } | True si les données externes récupérées via la connexion pour remplir un tableau doivent être enregistrées avec le classeur ; sinon, false.(Hérité de [`ExternalConnection`](../externalconnection/).) |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword/) { get; set; } | True si le mot de passe doit être enregistré dans la chaîne de connexion ; sinon, False. |
| virtual [SecondCommand](../../aspose.cells.externalconnections/externalconnection/secondcommand/) { get; set; } | Spécifie une deuxième chaîne de texte de commande qui est conservée lorsque les champs de page basés sur le serveur du tableau croisé dynamique sont utilisés. Pour les connexions ODBC, serverCommand est généralement une requête plus large que command (aucune clause WHERE n'est présente dans la première). En se basant sur ces 2 commandes (Command et ServerCommand), l'interface utilisateur des paramètres peut être remplie et des requêtes paramétrées peuvent être construites (Hérité de [`ExternalConnection`](../externalconnection/).) |
| [SourceFile](../../aspose.cells.externalconnections/externalconnection/sourcefile/) { get; set; } | Utilisé lorsque la source de données externe est basée sur un fichier. Lorsqu’une connexion à une telle source de données échoue, l’application de feuille de calcul tente de se connecter directement à ce fichier. Peut être exprimé sous forme d’URI ou de notation de chemin de fichier spécifique au système.(Hérité de [`ExternalConnection`](../externalconnection/).) |
| [SourceType](../../aspose.cells.externalconnections/externalconnection/sourcetype/) { get; set; } | Obtient ou définit le type DataSource de la connexion externe.(Hérité de [`ExternalConnection`](../externalconnection/).) |
| [SSOId](../../aspose.cells.externalconnections/externalconnection/ssoid/) { get; set; } | Identifiant pour l’authentification Single Sign On (SSO) utilisée entre un serveur intermédiaire spreadsheetML et la source de données externe.(Hérité de [`ExternalConnection`](../externalconnection/).) |
| [Type](../../aspose.cells.externalconnections/externalconnection/type/) { get; set; } | (**Obsolete.**) Obtient ou définit le type DataSource de la connexion externe.(Hérité de [`ExternalConnection`](../externalconnection/).) |
| [Url](../../aspose.cells.externalconnections/webqueryconnection/url/) { get; set; } | URL à utiliser pour actualiser les données externes. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassWebQueryConnectionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();

            try
            {
                // Créer une connexion de requête Web via la collection
                WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[workbook.DataConnections.Count];
                
                connection.Url = "https://example.com/financial-data";
                connection.IsHtmlTables = true;
                connection.IsTextDates = true;
                connection.HtmlFormat = HtmlFormatHandlingType.All;

                Console.WriteLine($"Web query URL: {connection.Url}");
                Console.WriteLine($"HTML tables only: {connection.IsHtmlTables}");

                workbook.Save("WebQueryConnectionDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with WebQueryConnection: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [ExternalConnection](../externalconnection/)
* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


