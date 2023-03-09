---
title: WebQueryConnection classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 70
url: /fr/python-net/aspose.cells.externalconnections/webqueryconnection/
is_root: false
---
##  WebQueryConnection classe
 Spécifie les propriétés d'une source de requête Web. Une requête Web récupérera les données de HTML tables,
 et peut également fournir des paramètres HTTP "Get" à traiter par le serveur Web lors de la génération du HTML par
y compris les paramètres et les éléments de paramètre.



**Héritage:** [WebQueryConnection](/cells/python-net/aspose.cells.externalconnections/webqueryconnection) → 
[ExternalConnection](/cells/fr/python-net/aspose.cells.externalconnections/externalconnection)



Le type WebQueryConnection expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [id](/cells/fr/python-net/aspose.cells.externalconnections/webqueryconnection/id) | Obtient l'identifiant de la connexion.|
| [power_query_formula](/cells/fr/python-net/aspose.cells.externalconnections/webqueryconnection/power_query_formula) | Obtient la définition de la formule de requête de puissance.|
| [type](/cells/fr/python-net/aspose.cells.externalconnections/webqueryconnection/type) | Obtient ou définit le type de source de données de la connexion externe.|
| [source_file](/cells/fr/python-net/aspose.cells.externalconnections/webqueryconnection/source_file) | Utilisé lorsque la source de données externe est basée sur un fichier. Lorsqu'une connexion à de telles données<br/> source échoue, le tableur tente de se connecter directement à ce fichier. Peut être<br/> exprimé en URI ou en notation de chemin de fichier spécifique au système.|
| [sso_id](/cells/fr/python-net/aspose.cells.externalconnections/webqueryconnection/sso_id) | Identifiant pour Single Sign On (SSO) utilisé pour l'authentification entre un intermédiaire<br/>serveur spreadsheetML et la source de données externe.|
| [save_password](/cells/fr/python-net/aspose.cells.externalconnections/webqueryconnection/save_password) |True si le mot de passe doit être enregistré dans le cadre de la chaîne de connexion ; sinon, Faux.|
| [save_data](/cells/fr/python-net/aspose.cells.externalconnections/webqueryconnection/save_data) | Vrai si les données externes récupérées via la connexion pour remplir une table doivent être enregistrées<br/> avec le cahier d'exercices; sinon, faux.|
| [refresh_on_load](/cells/fr/python-net/aspose.cells.externalconnections/webqueryconnection/refresh_on_load) | Vrai si cette connexion doit être actualisée lors de l'ouverture du fichier ; sinon, faux.|
| [reconnection_method_type](/cells/fr/python-net/aspose.cells.externalconnections/webqueryconnection/reconnection_method_type) | Spécifie ce que l'application de feuille de calcul doit faire lorsqu'une connexion échoue.<br/> La valeur par défaut est ReConnectionMethodType.Required.|
| [reconnection_method](/cells/fr/python-net/aspose.cells.externalconnections/webqueryconnection/reconnection_method) | Spécifie ce que l'application de feuille de calcul doit faire lorsqu'une connexion échoue.<br/> La valeur par défaut est ReConnectionMethodType.Required.|
| [only_use_connection_file](/cells/fr/python-net/aspose.cells.externalconnections/webqueryconnection/only_use_connection_file) | Indique si le tableur doit toujours et uniquement utiliser le<br/> informations de connexion dans le fichier de connexion externe indiqué par l'attribut odcFile<br/> lorsque la connexion est actualisée. Si false, alors l'application de feuille de calcul<br/> doit suivre la procédure indiquée par l'attribut reconnectionMethod|
| [odc_file](/cells/fr/python-net/aspose.cells.externalconnections/webqueryconnection/odc_file) | Spécifie le chemin d'accès complet au fichier de connexion externe à partir duquel cette connexion a été<br/> créé. Si une connexion échoue lors d'une tentative d'actualisation des données et que reconnectionMethod=1,<br/> puis l'application de feuille de calcul essaiera à nouveau en utilisant les informations du fichier de connexion externe<br/> au lieu de l'objet de connexion incorporé dans le classeur.|
| [is_new](/cells/fr/python-net/aspose.cells.externalconnections/webqueryconnection/is_new) | True si la connexion n'a pas été actualisée pour la première fois ; sinon, faux.<br/> Cet état peut se produire lorsque l'utilisateur enregistre le fichier avant qu'une requête n'ait fini de renvoyer.|
| [name](/cells/fr/python-net/aspose.cells.externalconnections/webqueryconnection/name) | Spécifie le nom de la connexion. Chaque connexion doit avoir un nom unique.|
| [keep_alive](/cells/fr/python-net/aspose.cells.externalconnections/webqueryconnection/keep_alive) | Vrai lorsque l'application de feuille de calcul doit faire des efforts pour maintenir la connexion<br/> ouvrir. Si false, l'application doit fermer la connexion après avoir récupéré le<br/> information.|
| [refresh_internal](/cells/fr/python-net/aspose.cells.externalconnections/webqueryconnection/refresh_internal) | Spécifie le nombre de minutes entre les actualisations automatiques de la connexion.|
| [connection_id](/cells/fr/python-net/aspose.cells.externalconnections/webqueryconnection/connection_id) | Spécifie l'identifiant unique de cette connexion.|
| [connection_description](/cells/fr/python-net/aspose.cells.externalconnections/webqueryconnection/connection_description) | Spécifie la description de l'utilisateur pour cette connexion|
| [is_deleted](/cells/fr/python-net/aspose.cells.externalconnections/webqueryconnection/is_deleted) | Indique si la connexion de classeur associée a été supprimée. vrai si le<br/> la connexion a été supprimée ; sinon, faux.|
| [credentials_method_type](/cells/fr/python-net/aspose.cells.externalconnections/webqueryconnection/credentials_method_type) | Spécifie la méthode d'authentification à utiliser lors de l'établissement (ou du rétablissement) de la connexion.|
| [credentials](/cells/fr/python-net/aspose.cells.externalconnections/webqueryconnection/credentials) | Spécifie la méthode d'authentification à utiliser lors de l'établissement (ou du rétablissement) de la connexion.|
| [background_refresh](/cells/fr/python-net/aspose.cells.externalconnections/webqueryconnection/background_refresh) | Indique si la connexion peut être actualisée en arrière-plan (de manière asynchrone).<br/> true si l'utilisation préférée de la connexion consiste à actualiser de manière asynchrone en arrière-plan ;<br/>false si l'utilisation préférée de la connexion consiste à actualiser de manière synchrone au premier plan.|
| [parameters](/cells/fr/python-net/aspose.cells.externalconnections/webqueryconnection/parameters) | Obtient [ConnectionParameterCollection](/cells/fr/python-net/aspose.cells.externalconnections/connectionparametercollection) pour une requête ODBC ou Web.|
| [is_xml](/cells/fr/python-net/aspose.cells.externalconnections/webqueryconnection/is_xml) | true si la source de la requête Web est XML (versus HTML), sinon false.|
| [is_xl97](/cells/fr/python-net/aspose.cells.externalconnections/webqueryconnection/is_xl97) | Cet indicateur existe pour la rétrocompatibilité avec les anciens fichiers de feuille de calcul existants et est défini<br/>à vrai si cette requête Web a été créée dans Microsoft Excel 97.<br/> Il s'agit d'un attribut facultatif qui peut être ignoré.|
| [is_xl2000](/cells/fr/python-net/aspose.cells.externalconnections/webqueryconnection/is_xl2000) | Cet indicateur existe pour la rétrocompatibilité avec les anciens fichiers de feuille de calcul existants et est défini<br/>à vrai si cette requête Web a été actualisée dans une application de feuille de calcul plus récente ou égale<br/>au Microsoft Excel 2000.<br/> Il s'agit d'un attribut facultatif qui peut être ignoré.|
| [url](/cells/fr/python-net/aspose.cells.externalconnections/webqueryconnection/url) | URL à utiliser pour actualiser les données externes.|
| [is_text_dates](/cells/fr/python-net/aspose.cells.externalconnections/webqueryconnection/is_text_dates) | Indicateur indiquant si les dates doivent être importées dans les cellules de la feuille de calcul sous forme de texte plutôt que de dates.|
| [is_xml_source_data](/cells/fr/python-net/aspose.cells.externalconnections/webqueryconnection/is_xml_source_data) | Indicateur indiquant que les données source XML doivent être importées à la place de la table HTML elle-même.|
| [post](/cells/fr/python-net/aspose.cells.externalconnections/webqueryconnection/post) | Renvoie ou définit la chaîne utilisée avec la méthode post de saisie de données dans un serveur Web<br/> pour renvoyer des données à partir d'une requête Web.|
| [is_parse_pre](/cells/fr/python-net/aspose.cells.externalconnections/webqueryconnection/is_parse_pre) |Indicateur indiquant si les données contenues dans les balises HTML PRE de la page Web sont<br/> analysés en colonnes lorsque vous importez la page dans une table de requête.|
| [is_html_tables](/cells/fr/python-net/aspose.cells.externalconnections/webqueryconnection/is_html_tables) | Indicateur indiquant si les requêtes Web ne doivent fonctionner que sur les tables HTML.|
| [html_format](/cells/fr/python-net/aspose.cells.externalconnections/webqueryconnection/html_format) | Comment gérer le formatage à partir de la source HTML lors de l'importation de données de requête Web dans le<br/> feuille de travail. Pertinent lorsque sourceData est True.|
| [is_same_settings](/cells/fr/python-net/aspose.cells.externalconnections/webqueryconnection/is_same_settings) | Drapeau indiquant s'il faut analyser toutes les tables à l'intérieur d'un bloc PRE avec les mêmes paramètres de largeur<br/> comme première rangée.|
| [edit_web_page](/cells/fr/python-net/aspose.cells.externalconnections/webqueryconnection/edit_web_page) | L'URL de la page Web accessible à l'utilisateur affichant les données de la requête Web. Cette URL est persistante<br/>dans le cas où sourceData="true" et url ont été redirigés pour référencer un fichier XML.<br/>Ensuite, la page destinée à l'utilisateur peut être affichée dans l'interface utilisateur et les données XML peuvent être récupérées<br/> Dans les coulisses.|
| [edit_page](/cells/fr/python-net/aspose.cells.externalconnections/webqueryconnection/edit_page) | L'URL de la page Web accessible à l'utilisateur affichant les données de la requête Web. Cette URL est persistante<br/>dans le cas où sourceData="true" et url ont été redirigés pour référencer un fichier XML.<br/>Ensuite, la page destinée à l'utilisateur peut être affichée dans l'interface utilisateur et les données XML peuvent être récupérées<br/> Dans les coulisses.|
| [is_consecutive](/cells/fr/python-net/aspose.cells.externalconnections/webqueryconnection/is_consecutive) | Indicateur indiquant si des délimiteurs consécutifs doivent être traités comme un seul délimiteur.|



###  Voir également
* module [aspose.cells.externalconnections](..)
* classe [ConnectionParameterCollection](/cells/fr/python-net/aspose.cells.externalconnections/connectionparametercollection)
* classe [ExternalConnection](/cells/fr/python-net/aspose.cells.externalconnections/externalconnection)
* classe [WebQueryConnection](/cells/fr/python-net/aspose.cells.externalconnections/webqueryconnection)
