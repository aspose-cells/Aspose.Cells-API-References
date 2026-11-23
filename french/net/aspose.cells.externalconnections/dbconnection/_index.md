---
title: "Classe DBConnection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.ExternalConnections.DBConnection. Spécifie toutes les propriétés associées à une connexion de données externes ODBC ou OLE DB."
type: docs
url: /fr/net/aspose.cells.externalconnections/dbconnection/
---
## DBConnection class

Spécifie toutes les propriétés associées à une connexion de données externes ODBC ou OLE DB.

```csharp
public class DBConnection : ExternalConnection
```

## Propriétés

| Nom | Description |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh/) { get; set; } | Indique si la connexion peut être rafraîchie en arrière-plan (asynchroniquement). true si l’utilisation préférée de la connexion est de rafraîchir de façon asynchrone en arrière-plan ; false si l’utilisation préférée de la connexion est de rafraîchir de façon synchrone au premier plan.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| override [ClassType](../../aspose.cells.externalconnections/dbconnection/classtype/) { get; } | Obtient le type de cet objet [`ExternalConnection`](../externalconnection/). |
| override [Command](../../aspose.cells.externalconnections/dbconnection/command/) { get; set; } | La chaîne contenant la commande de base de données à transmettre à l’API du fournisseur de données qui interagira avec la source externe afin de récupérer les données |
| override [CommandType](../../aspose.cells.externalconnections/dbconnection/commandtype/) { get; set; } | Spécifie le type de commande OLE DB. 1. Query spécifie un nom de cube 2. Query spécifie une instruction SQL 3. Query spécifie un nom de table 4. Query spécifie que des informations par défaut ont été fournies, et il revient au fournisseur de les interpréter. 5. Query porte sur un fournisseur de données de liste basé sur le web. |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription/) { get; set; } | Spécifie la description utilisateur pour cette connexion(Inherited from [`ExternalConnection`](../externalconnection/).) |
| virtual [ConnectionFile](../../aspose.cells.externalconnections/externalconnection/connectionfile/) { get; } | Obtient le fichier de connexion.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid/) { get; } | (**Obsolete.**) Spécifie l’identifiant unique de cette connexion.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [ConnectionInfo](../../aspose.cells.externalconnections/dbconnection/connectioninfo/) { get; set; } | (**Obsolete.**) La chaîne d’informations de connexion est utilisée pour établir le contact avec une source de données OLE DB ou ODBC. |
| override [ConnectionString](../../aspose.cells.externalconnections/dbconnection/connectionstring/) { get; set; } | La chaîne d’informations de connexion est utilisée pour établir le contact avec une source de données OLE DB ou ODBC. |
| [Credentials](../../aspose.cells.externalconnections/externalconnection/credentials/) { get; set; } | (**Obsolete.**) Spécifie la méthode d’authentification à utiliser lors de l’établissement (ou du ré‑établissement) de la connexion.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype/) { get; set; } | Spécifie la méthode d’authentification à utiliser lors de l’établissement (ou du ré‑établissement) de la connexion.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [Id](../../aspose.cells.externalconnections/externalconnection/id/) { get; } | Obtient l’identifiant de la connexion.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted/) { get; set; } | Indique si la connexion de classeur associée a été supprimée. true si la connexion a été supprimée ; sinon, false.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew/) { get; set; } | True si la connexion n’a pas été rafraîchie pour la première fois ; sinon, false. Cet état peut se produire lorsque l’utilisateur enregistre le fichier avant qu’une requête ne soit terminée.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive/) { get; set; } | True lorsque l’application de feuille de calcul doit s’efforcer de garder la connexion ouverte. false lorsque l’application doit fermer la connexion après avoir récupéré les informations.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [Name](../../aspose.cells.externalconnections/externalconnection/name/) { get; set; } | Spécifie le nom de la connexion. Chaque connexion doit avoir un nom unique.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile/) { get; set; } | Spécifie le chemin complet du fichier de connexion externe à partir duquel cette connexion a été créée. Si une connexion échoue lors d’une tentative de rafraîchissement des données, et reconnectionMethod=1, alors l’application de feuille de calcul réessaiera en utilisant les informations du fichier de connexion externe au lieu de l’objet de connexion intégré dans le classeur.(Hérité de [`ExternalConnection`](../externalconnection/).) |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile/) { get; set; } | Indique si l’application de feuille de calcul doit toujours et uniquement utiliser les informations de connexion du fichier de connexion externe indiqué par l’attribut odcFile lors du rafraîchissement de la connexion. Si false, alors l’application de feuille de calcul doit suivre la procédure indiquée par l’attribut reconnectionMethod.(Hérité de [`ExternalConnection`](../externalconnection/).) |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters/) { get; } | Obtient [`ConnectionParameterCollection`](../connectionparametercollection/) pour une requête ODBC ou Web.(Hérité de [`ExternalConnection`](../externalconnection/).) |
| override [PowerQueryFormula](../../aspose.cells.externalconnections/dbconnection/powerqueryformula/) { get; } | Obtient la définition de la formule Power Query. |
| [ReconnectionMethod](../../aspose.cells.externalconnections/externalconnection/reconnectionmethod/) { get; set; } | (**Obsolete.**) Spécifie ce que l’application de feuille de calcul doit faire lorsqu’une connexion échoue. La valeur par défaut est ReConnectionMethodType.Required.(Hérité de [`ExternalConnection`](../externalconnection/).) |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype/) { get; set; } | Spécifie ce que l’application de feuille de calcul doit faire lorsqu’une connexion échoue. La valeur par défaut est ReConnectionMethodType.Required.(Hérité de [`ExternalConnection`](../externalconnection/).) |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal/) { get; set; } | Spécifie le nombre de minutes entre les rafraîchissements automatiques de la connexion.(Hérité de [`ExternalConnection`](../externalconnection/).) |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload/) { get; set; } | True si cette connexion doit être rafraîchie à l’ouverture du fichier ; sinon, false.(Hérité de [`ExternalConnection`](../externalconnection/).) |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata/) { get; set; } | True si les données externes récupérées via la connexion pour remplir un tableau doivent être enregistrées avec le classeur ; sinon, false.(Hérité de [`ExternalConnection`](../externalconnection/).) |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword/) { get; set; } | True si le mot de passe doit être enregistré dans la chaîne de connexion ; sinon, False. |
| override [SecondCommand](../../aspose.cells.externalconnections/dbconnection/secondcommand/) { get; set; } | Spécifie une deuxième chaîne de texte de commande qui est conservée lorsque les champs de page basés sur le serveur du tableau croisé dynamique sont utilisés. Pour les connexions ODBC, serverCommand est généralement une requête plus large que command (aucune clause WHERE n’est présente dans la première). En se basant sur ces 2 commandes (Command et ServerCommand), l’interface utilisateur des paramètres peut être remplie et des requêtes paramétrées peuvent être construites |
| [SeverCommand](../../aspose.cells.externalconnections/dbconnection/severcommand/) { get; set; } | (**Obsolete.**) Spécifie une deuxième chaîne de texte de commande qui est conservée lorsque les champs de page basés sur le serveur du tableau croisé dynamique sont utilisés. Pour les connexions ODBC, serverCommand est généralement une requête plus large que command (aucune clause WHERE n’est présente dans la première). En se basant sur ces 2 commandes (Command et ServerCommand), l’interface utilisateur des paramètres peut être remplie et des requêtes paramétrées peuvent être construites |
| [SourceFile](../../aspose.cells.externalconnections/externalconnection/sourcefile/) { get; set; } | Utilisé lorsque la source de données externe est basée sur un fichier. Lorsqu’une connexion à une telle source de données échoue, l’application de feuille de calcul tente de se connecter directement à ce fichier. Peut être exprimé sous forme d’URI ou de notation de chemin de fichier spécifique au système.(Hérité de [`ExternalConnection`](../externalconnection/).) |
| [SourceType](../../aspose.cells.externalconnections/externalconnection/sourcetype/) { get; set; } | Obtient ou définit le type DataSource de la connexion externe.(Hérité de [`ExternalConnection`](../externalconnection/).) |
| [SSOId](../../aspose.cells.externalconnections/externalconnection/ssoid/) { get; set; } | Identifiant pour l’authentification Single Sign On (SSO) utilisée entre un serveur intermédiaire spreadsheetML et la source de données externe.(Hérité de [`ExternalConnection`](../externalconnection/).) |
| [Type](../../aspose.cells.externalconnections/externalconnection/type/) { get; set; } | (**Obsolete.**) Obtient ou définit le type DataSource de la connexion externe.(Hérité de [`ExternalConnection`](../externalconnection/).) |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassDBConnectionDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Créez une nouvelle instance DBConnection en l’ajoutant à la collection
                var connections = workbook.DataConnections;
                DBConnection dbConnection = (DBConnection)connections[connections.Count];

                // Définir les propriétés de base
                dbConnection.ConnectionString = "Provider=Microsoft.Jet.OLEDB.4.0;Data Source=C:\\data\\database.mdb;";
                dbConnection.CommandType = OLEDBCommandType.TableName;
                dbConnection.Command = "Customers";

                // Afficher les propriétés en lecture seule
                Console.WriteLine("DBConnection ClassType: " + dbConnection.ClassType);
                Console.WriteLine("ConnectionString: " + dbConnection.ConnectionString);
                Console.WriteLine("CommandType: " + dbConnection.CommandType);
                Console.WriteLine("Command: " + dbConnection.Command);

                // Enregistrez le classeur
                workbook.Save("DBConnectionDemo.xlsx");
                Console.WriteLine("DBConnection demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with DBConnection: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [ExternalConnection](../externalconnection/)
* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


