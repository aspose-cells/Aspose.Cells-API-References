---
title: "Classe ExternalConnection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.ExternalConnections.ExternalConnection. Spécifie une connexion de données externe"
type: docs
url: /fr/net/aspose.cells.externalconnections/externalconnection/
---
## ExternalConnection class

Spécifie une connexion de données externes

```csharp
public abstract class ExternalConnection
```

## Propriétés

| Nom | Description |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh/) { get; set; } | Indique si la connexion peut être actualisée en arrière‑plan (asynchrone). true si l’utilisation préférée de la connexion est de rafraîchir de façon asynchrone en arrière‑plan ; false si l’utilisation préférée est de rafraîchir de façon synchrone au premier plan. |
| abstract [ClassType](../../aspose.cells.externalconnections/externalconnection/classtype/) { get; } | Obtient le type de cet objet `ExternalConnection`. |
| virtual [Command](../../aspose.cells.externalconnections/externalconnection/command/) { get; set; } | La chaîne contenant la commande de base de données à transmettre à l’API du fournisseur de données qui interagira avec la source externe afin de récupérer les données |
| virtual [CommandType](../../aspose.cells.externalconnections/externalconnection/commandtype/) { get; set; } | Spécifie le type de commande OLE DB. 1. Query spécifie un nom de cube 2. Query spécifie une instruction SQL 3. Query spécifie un nom de table 4. Query spécifie que des informations par défaut ont été fournies, et il revient au fournisseur de les interpréter. 5. Query porte sur un fournisseur de données de liste basé sur le web. |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription/) { get; set; } | Spécifie la description utilisateur pour cette connexion |
| virtual [ConnectionFile](../../aspose.cells.externalconnections/externalconnection/connectionfile/) { get; } | Obtient le fichier de connexion. |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid/) { get; } | (**Obsolete.**) Spécifie l’identifiant unique de cette connexion. |
| virtual [ConnectionString](../../aspose.cells.externalconnections/externalconnection/connectionstring/) { get; set; } | La chaîne d’informations de connexion est utilisée pour établir le contact avec une source de données OLE DB ou ODBC. |
| [Credentials](../../aspose.cells.externalconnections/externalconnection/credentials/) { get; set; } | (**Obsolete.**) Spécifie la méthode d’authentification à utiliser lors de l’établissement (ou du ré‑établissement) de la connexion. |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype/) { get; set; } | Spécifie la méthode d’authentification à utiliser lors de l’établissement (ou du ré‑établissement) de la connexion. |
| [Id](../../aspose.cells.externalconnections/externalconnection/id/) { get; } | Obtient l’identifiant de la connexion. |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted/) { get; set; } | Indique si la connexion de classeur associée a été supprimée. true si la connexion a été supprimée ; sinon false. |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew/) { get; set; } | True si la connexion n’a pas encore été actualisée pour la première fois ; sinon false. Cet état peut se produire lorsque l’utilisateur enregistre le fichier avant que la requête ne se termine. |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive/) { get; set; } | True lorsque l’application de feuille de calcul doit s’efforcer de garder la connexion ouverte. Lorsque false, l’application doit fermer la connexion après avoir récupéré les informations. |
| [Name](../../aspose.cells.externalconnections/externalconnection/name/) { get; set; } | Spécifie le nom de la connexion. Chaque connexion doit avoir un nom unique. |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile/) { get; set; } | Spécifie le chemin complet vers le fichier de connexion externe à partir duquel cette connexion a été créée. Si une connexion échoue lors d’une tentative d’actualisation des données, et reconnectionMethod=1, alors l’application de feuille de calcul réessaiera en utilisant les informations du fichier de connexion externe au lieu de l’objet de connexion intégré au classeur. |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile/) { get; set; } | Indique si l’application de feuille de calcul doit toujours et uniquement utiliser les informations de connexion du fichier de connexion externe indiqué par l’attribut odcFile lors de l’actualisation de la connexion. Si false, alors l’application de feuille de calcul doit suivre la procédure indiquée par l’attribut reconnectionMethod. |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters/) { get; } | Obtient [`ConnectionParameterCollection`](../connectionparametercollection/) pour une requête ODBC ou Web. |
| virtual [PowerQueryFormula](../../aspose.cells.externalconnections/externalconnection/powerqueryformula/) { get; } | Obtient la définition de la formule Power Query. |
| [ReconnectionMethod](../../aspose.cells.externalconnections/externalconnection/reconnectionmethod/) { get; set; } | (**Obsolete.**) Spécifie ce que l’application de feuille de calcul doit faire lorsqu’une connexion échoue. La valeur par défaut est ReConnectionMethodType.Required. |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype/) { get; set; } | Spécifie ce que l’application de feuille de calcul doit faire lorsqu’une connexion échoue. La valeur par défaut est ReConnectionMethodType.Required. |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal/) { get; set; } | Spécifie le nombre de minutes entre les rafraîchissements automatiques de la connexion. |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload/) { get; set; } | Vrai si cette connexion doit être rafraîchie lors de l'ouverture du fichier ; sinon, faux. |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata/) { get; set; } | Vrai si les données externes récupérées via la connexion pour remplir un tableau doivent être enregistrées avec le classeur ; sinon, faux. |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword/) { get; set; } | Vrai si le mot de passe doit être enregistré dans la chaîne de connexion ; sinon, Faux. |
| virtual [SecondCommand](../../aspose.cells.externalconnections/externalconnection/secondcommand/) { get; set; } | Spécifie une deuxième chaîne de texte de commande qui est conservée lorsque les champs de page basés sur le serveur du tableau croisé dynamique sont utilisés. Pour les connexions ODBC, serverCommand est généralement une requête plus large que command (aucune clause WHERE n’est présente dans la première). En se basant sur ces 2 commandes (Command et ServerCommand), l’interface utilisateur des paramètres peut être remplie et des requêtes paramétrées peuvent être construites |
| [SourceFile](../../aspose.cells.externalconnections/externalconnection/sourcefile/) { get; set; } | Utilisé lorsque la source de données externe est basée sur un fichier. Lorsqu'une connexion à une telle source de données échoue, l'application de feuille de calcul tente de se connecter directement à ce fichier. Peut être exprimé en URI ou en notation de chemin de fichier spécifique au système. |
| [SourceType](../../aspose.cells.externalconnections/externalconnection/sourcetype/) { get; set; } | Obtient ou définit le type DataSource de la connexion externe. |
| [SSOId](../../aspose.cells.externalconnections/externalconnection/ssoid/) { get; set; } | Identifiant pour Single Sign On (SSO) utilisé pour l'authentification entre un serveur intermédiaire spreadsheetML et la source de données externe. |
| [Type](../../aspose.cells.externalconnections/externalconnection/type/) { get; set; } | (**Obsolete.**) Obtient ou définit le type DataSource de la connexion externe. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionsClassExternalConnectionDemo
    {
        public static void Run()
        {
            string sourceDir = "Your Source Directory";

            Workbook workbook = new Workbook(sourceDir + "example.xlsx");
            ExternalConnectionCollection conns = workbook.DataConnections;
            foreach (ExternalConnection conn in conns)
            {
                if (conn is DBConnection dbConn)
                {
                    Console.WriteLine("Connection Info: " + dbConn.ConnectionInfo);
                    Console.WriteLine("Formula Definition: " + dbConn.PowerQueryFormula.FormulaDefinition);
                }
            }

            workbook = new Workbook(sourceDir + "example.xlsm");
            conns = workbook.DataConnections;
            foreach (ExternalConnection conn in conns)
            {
                if (conn is DBConnection dbConn)
                {
                    Console.WriteLine("Connection Info: " + dbConn.ConnectionInfo);
                    Console.WriteLine("Formula Definition: " + dbConn.PowerQueryFormula.FormulaDefinition);
                }
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


