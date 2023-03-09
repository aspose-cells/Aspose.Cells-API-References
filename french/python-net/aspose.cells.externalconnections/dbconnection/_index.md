---
title: DBConnection classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 30
url: /fr/python-net/aspose.cells.externalconnections/dbconnection/
is_root: false
---
##  DBConnection classe
Spécifie toutes les propriétés associées à une connexion de données externes ODBC ou OLE DB.



**Héritage:** [DBConnection](/cells/python-net/aspose.cells.externalconnections/dbconnection) → 
[ExternalConnection](/cells/fr/python-net/aspose.cells.externalconnections/externalconnection)



Le type DBConnection expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [id](/cells/fr/python-net/aspose.cells.externalconnections/dbconnection/id) | Obtient l'identifiant de la connexion.|
| [power_query_formula](/cells/fr/python-net/aspose.cells.externalconnections/dbconnection/power_query_formula) | Obtient la définition de la formule de requête de puissance.|
| [type](/cells/fr/python-net/aspose.cells.externalconnections/dbconnection/type) | Obtient ou définit le type de source de données de la connexion externe.|
| [source_file](/cells/fr/python-net/aspose.cells.externalconnections/dbconnection/source_file) | Utilisé lorsque la source de données externe est basée sur un fichier.<br/> source échoue, le tableur tente de se connecter directement à ce fichier.<br/> exprimé en URI ou en notation de chemin de fichier spécifique au système.|
| [sso_id](/cells/fr/python-net/aspose.cells.externalconnections/dbconnection/sso_id) | Identifiant pour Single Sign On (SSO) utilisé pour l'authentification entre un intermédiaire<br/> serveur spreadsheetML et la source de données externe.|
| [save_password](/cells/fr/python-net/aspose.cells.externalconnections/dbconnection/save_password) | True si le mot de passe doit être enregistré dans le cadre de la chaîne de connexion ; sinon, False.|
| [save_data](/cells/fr/python-net/aspose.cells.externalconnections/dbconnection/save_data) | Vrai si les données externes récupérées via la connexion pour remplir une table doivent être enregistrées<br/> avec le classeur ; sinon, faux.|
| [refresh_on_load](/cells/fr/python-net/aspose.cells.externalconnections/dbconnection/refresh_on_load) | Vrai si cette connexion doit être actualisée lors de l'ouverture du fichier ;|
| [reconnection_method_type](/cells/fr/python-net/aspose.cells.externalconnections/dbconnection/reconnection_method_type) | Spécifie ce que l'application de feuille de calcul doit faire lorsqu'une connexion échoue.<br/>La valeur par défaut est ReConnectionMethodType.Required.|
| [reconnection_method](/cells/fr/python-net/aspose.cells.externalconnections/dbconnection/reconnection_method) | Spécifie ce que l'application de feuille de calcul doit faire lorsqu'une connexion échoue.<br/>La valeur par défaut est ReConnectionMethodType.Required.|
| [only_use_connection_file](/cells/fr/python-net/aspose.cells.externalconnections/dbconnection/only_use_connection_file) | Indique si le tableur doit toujours et uniquement utiliser le<br/> informations de connexion dans le fichier de connexion externe indiqué par l'attribut odcFile<br/> lors de l'actualisation de la connexion. Si false, l'application de tableur<br/> doit suivre la procédure indiquée par l'attribut reconnectionMethod|
| [odc_file](/cells/fr/python-net/aspose.cells.externalconnections/dbconnection/odc_file) | Spécifie le chemin d'accès complet au fichier de connexion externe à partir duquel cette connexion a été<br/> Si une connexion échoue lors d'une tentative d'actualisation des données et que reconnectionMethod=1,<br/> puis l'application de feuille de calcul essaiera à nouveau en utilisant les informations du fichier de connexion externe<br/> au lieu de l'objet de connexion incorporé dans le classeur.|
| [is_new](/cells/fr/python-net/aspose.cells.externalconnections/dbconnection/is_new) | Vrai si la connexion n'a pas été actualisée pour la première fois ; sinon, faux.<br/> Cet état peut se produire lorsque l'utilisateur enregistre le fichier avant qu'une requête n'ait fini de renvoyer.|
| [name](/cells/fr/python-net/aspose.cells.externalconnections/dbconnection/name) | Spécifie le nom de la connexion.|
| [keep_alive](/cells/fr/python-net/aspose.cells.externalconnections/dbconnection/keep_alive) | Vrai lorsque l'application de feuille de calcul doit faire des efforts pour maintenir la connexion<br/>Si false, l'application doit fermer la connexion après avoir récupéré le<br/> information.|
| [refresh_internal](/cells/fr/python-net/aspose.cells.externalconnections/dbconnection/refresh_internal) | Spécifie le nombre de minutes entre les actualisations automatiques de la connexion.|
| [connection_id](/cells/fr/python-net/aspose.cells.externalconnections/dbconnection/connection_id) | Spécifie l'identifiant unique de cette connexion.|
| [connection_description](/cells/fr/python-net/aspose.cells.externalconnections/dbconnection/connection_description) | Spécifie la description de l'utilisateur pour cette connexion|
| [is_deleted](/cells/fr/python-net/aspose.cells.externalconnections/dbconnection/is_deleted) |Indique si la connexion au classeur associé a été supprimée. true si le<br/> sinon, faux.|
| [credentials_method_type](/cells/fr/python-net/aspose.cells.externalconnections/dbconnection/credentials_method_type) | Spécifie la méthode d'authentification à utiliser lors de l'établissement (ou du rétablissement) de la connexion.|
| [credentials](/cells/fr/python-net/aspose.cells.externalconnections/dbconnection/credentials) | Spécifie la méthode d'authentification à utiliser lors de l'établissement (ou du rétablissement) de la connexion.|
| [background_refresh](/cells/fr/python-net/aspose.cells.externalconnections/dbconnection/background_refresh) | Indique si la connexion peut être actualisée en arrière-plan (de manière asynchrone).<br/>true si l'utilisation préférée de la connexion consiste à actualiser de manière asynchrone en arrière-plan ;<br/> false si l'utilisation préférée de la connexion consiste à actualiser de manière synchrone au premier plan.|
| [parameters](/cells/fr/python-net/aspose.cells.externalconnections/dbconnection/parameters) | Obtient [ConnectionParameterCollection](/cells/fr/python-net/aspose.cells.externalconnections/connectionparametercollection) pour une requête ODBC ou Web.|
| [connection_info](/cells/fr/python-net/aspose.cells.externalconnections/dbconnection/connection_info) | La chaîne d'informations de connexion est utilisée pour établir un contact avec une source de données OLE DB ou ODBC.|
| [command_type](/cells/fr/python-net/aspose.cells.externalconnections/dbconnection/command_type) | Spécifie le type de commande OLE DB.<br/>1. La requête spécifie un nom de cube<br/>2. La requête spécifie une instruction SQL<br/>3. La requête spécifie un nom de table<br/>4. La requête spécifie que les informations par défaut ont été fournies, et c'est au fournisseur de décider comment les interpréter.<br/> 5. La requête porte sur un fournisseur de données de liste basé sur le Web.|
| [command](/cells/fr/python-net/aspose.cells.externalconnections/dbconnection/command) | La chaîne contenant la commande de base de données à transmettre au fournisseur de données API qui<br/> interagir avec la source externe afin de récupérer des données|
| [sever_command](/cells/fr/python-net/aspose.cells.externalconnections/dbconnection/sever_command) |Spécifie une deuxième chaîne de texte de commande qui est conservée lorsque le tableau croisé dynamique basé sur le serveur<br/> les champs de la page sont en cours d'utilisation.<br/> Pour les connexions ODBC, serverCommand est généralement une requête plus large que command (pas<br/>La clause WHERE est présente dans le premier).<br/> l'interface utilisateur des paramètres peut être remplie et des requêtes paramétrées peuvent être construites|



###  Voir également
* module [aspose.cells.externalconnections](..)
* classe [ConnectionParameterCollection](/cells/fr/python-net/aspose.cells.externalconnections/connectionparametercollection)
* classe [DBConnection](/cells/fr/python-net/aspose.cells.externalconnections/dbconnection)
* classe [ExternalConnection](/cells/fr/python-net/aspose.cells.externalconnections/externalconnection)
