---
title: ConnectionParameter classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 10
url: /fr/python-net/aspose.cells.externalconnections/connectionparameter/
is_root: false
---
##  ConnectionParameter classe
Spécifie les propriétés de tous les paramètres utilisés avec les connexions de données externes
Les paramètres sont valides pour les requêtes ODBC et Web.



Le type ConnectionParameter expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [sql_type](/cells/fr/python-net/aspose.cells.externalconnections/connectionparameter/sql_type) | Type de données SQL du paramètre. Valable uniquement pour les sources ODBC.|
| [refresh_on_change](/cells/fr/python-net/aspose.cells.externalconnections/connectionparameter/refresh_on_change) | Indicateur indiquant si la requête doit se rafraîchir automatiquement lorsque le contenu d'un<br/> cellule qui fournit les changements de valeur de paramètre. Si vrai, les données externes sont actualisées<br/> en utilisant la nouvelle valeur de paramètre chaque fois qu'il y a un changement. Si faux, alors données externes<br/> n'est actualisé qu'à la demande de l'utilisateur, ou un autre événement déclenche l'actualisation (par exemple, classeur ouvert).|
| [prompt](/cells/fr/python-net/aspose.cells.externalconnections/connectionparameter/prompt) | Chaîne d'invite pour le paramètre. Présenté à l'utilisateur de la feuille de calcul avec l'interface utilisateur d'entrée<br/> pour collecter la valeur du paramètre avant d'actualiser les données externes. Utilisé uniquement lorsque<br/> paramètreType = invite.|
| [type](/cells/fr/python-net/aspose.cells.externalconnections/connectionparameter/type) | Type de paramètre utilisé.<br/>Si le type de paramètre=valeur, alors la valeur parmi booléen, double, entier,<br/> ou une chaîne sera utilisée. Dans ce cas, on s'attend à ce qu'un seul des<br/> {booléen, double, entier ou chaîne} sera spécifié.|
| [name](/cells/fr/python-net/aspose.cells.externalconnections/connectionparameter/name) | Le nom du paramètre.|
| [cell_reference](/cells/fr/python-net/aspose.cells.externalconnections/connectionparameter/cell_reference) | Cell référence indiquant quelle valeur de cellule utiliser pour le paramètre de requête. Utilisé uniquement lorsque parameterType est cell.|
| [value](/cells/fr/python-net/aspose.cells.externalconnections/connectionparameter/value) |Valeur numérique non entière, Valeur entière, Valeur chaîne ou Valeur booléenne<br/> à utiliser comme paramètre de requête. Utilisé uniquement lorsque parameterType est value.|



###  Voir également
* module [aspose.cells.externalconnections](..)
