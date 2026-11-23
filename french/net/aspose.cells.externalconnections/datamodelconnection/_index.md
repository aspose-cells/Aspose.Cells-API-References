---
title: "Classe DataModelConnection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.ExternalConnections.DataModelConnection. Spécifie une connexion de modèle de données"
type: docs
url: /fr/net/aspose.cells.externalconnections/datamodelconnection/
---
## DataModelConnection class

Spécifie une connexion de modèle de données

```csharp
public class DataModelConnection : ExternalConnection
```

## Propriétés

| Nom | Description |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh/) { get; set; } | Indique si la connexion peut être rafraîchie en arrière-plan (asynchroniquement). true si l’utilisation préférée de la connexion est de rafraîchir de façon asynchrone en arrière-plan ; false si l’utilisation préférée de la connexion est de rafraîchir de façon synchrone au premier plan.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| override [ClassType](../../aspose.cells.externalconnections/datamodelconnection/classtype/) { get; } | Obtient le type de cet objet [`ExternalConnection`](../externalconnection/). |
| override [Command](../../aspose.cells.externalconnections/datamodelconnection/command/) { get; set; } | La chaîne contenant la commande de base de données à transmettre à l’API du fournisseur de données qui interagira avec la source externe afin de récupérer les données |
| override [CommandType](../../aspose.cells.externalconnections/datamodelconnection/commandtype/) { get; set; } | Renvoie le type [`OLEDBCommandType`](../oledbcommandtype/). |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription/) { get; set; } | Spécifie la description utilisateur pour cette connexion(Inherited from [`ExternalConnection`](../externalconnection/).) |
| virtual [ConnectionFile](../../aspose.cells.externalconnections/externalconnection/connectionfile/) { get; } | Obtient le fichier de connexion.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid/) { get; } | (**Obsolete.**) Spécifie l’identifiant unique de cette connexion.(Inherited from [`ExternalConnection`](../externalconnection/).) |
| override [ConnectionString](../../aspose.cells.externalconnections/datamodelconnection/connectionstring/) { get; set; } | La chaîne d’informations de connexion est utilisée pour établir le contact avec une source de données OLE DB ou ODBC. |
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

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;
    using System.Collections.Generic;

    public class ExternalConnectionsClassDataModelConnectionDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();

            try
            {
                // Créer une instance de la classe DataModelConnection en utilisant la réflexion
                DataModelConnection connection = (DataModelConnection)System.Runtime.Serialization.FormatterServices.GetUninitializedObject(typeof(DataModelConnection));

                // Définissez les propriétés essentielles
                connection.Command = "SELECT * FROM Products";
                connection.CommandType = OLEDBCommandType.SqlStatement;
                connection.ConnectionString = "Provider=SQLOLEDB;Data Source=Northwind;Integrated Security=SSPI";

                // Ajouter la connexion aux connexions de données du classeur
                ((IList<ExternalConnection>)workbook.DataConnections).Add(connection);

                // Afficher les informations de connexion
                Console.WriteLine($"Connection Type: {connection.ClassType}");
                Console.WriteLine($"Command: {connection.Command}");
                Console.WriteLine($"Command Type: {connection.CommandType}");
                Console.WriteLine($"Connection String: {connection.ConnectionString}");

                // Enregistrez le classeur
                workbook.Save("DataModelConnectionDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with DataModelConnection.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with DataModelConnection: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [ExternalConnection](../externalconnection/)
* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


