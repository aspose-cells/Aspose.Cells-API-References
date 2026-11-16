---
title: "ConnectionParameter Classe"
linktitle: "ConnectionParameter"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "ConnectionParameter classe. Encapsule l'objet qui représente connectionparameter en Go."
type: docs
weight: 200
url: /fr/go-cpp/connectionparameter/
---

## ConnectionParameter class

Spécifie les propriétés concernant les paramètres utilisés avec les connexions de données externes. Les paramètres sont valides pour les requêtes ODBC et Web.

```go

type ConnectionParameter struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetSqlType](./getsqltype/) | Type de données SQL du paramètre. Valide uniquement pour les sources ODBC. |
| [SetSqlType](./setsqltype/) | Type de données SQL du paramètre. Valide uniquement pour les sources ODBC. |
| [GetRefreshOnChange](./getrefreshonchange/) | Flag indiquant si la requête doit se rafraîchir automatiquement lorsque le contenu d'une cellule qui fournit la valeur du paramètre change. Si true, alors les données externes sont rafraîchies en utilisant la nouvelle valeur du paramètre à chaque changement. Si false, alors les données externes ne sont rafraîchies que lorsqu'elles sont demandées par l'utilisateur, ou qu'un autre événement déclenche le rafraîchissement (par ex., classeur ouvert). |
| [SetRefreshOnChange](./setrefreshonchange/) | Flag indiquant si la requête doit se rafraîchir automatiquement lorsque le contenu d'une cellule qui fournit la valeur du paramètre change. Si true, alors les données externes sont rafraîchies en utilisant la nouvelle valeur du paramètre à chaque changement. Si false, alors les données externes ne sont rafraîchies que lorsqu'elles sont demandées par l'utilisateur, ou qu'un autre événement déclenche le rafraîchissement (par ex., classeur ouvert). |
| [GetPrompt](./getprompt/) | Chaîne d'invite pour le paramètre. Présentée à l'utilisateur de la feuille de calcul avec l'interface UI d'entrée pour collecter la valeur du paramètre avant de rafraîchir les données externes. Utilisée uniquement lorsque parameterType = prompt. |
| [SetPrompt](./setprompt/) | Chaîne d'invite pour le paramètre. Présentée à l'utilisateur de la feuille de calcul avec l'interface UI d'entrée pour collecter la valeur du paramètre avant de rafraîchir les données externes. Utilisée uniquement lorsque parameterType = prompt. |
| [GetType](./gettype/) | Type de paramètre utilisé. Si parameterType=value, alors la valeur provenant de boolean, double, integer ou string sera utilisée. Dans ce cas, il est attendu qu'une seule de {boolean, double, integer, or string} soit spécifiée. |
| [SetType](./settype/) | Type de paramètre utilisé. Si parameterType=value, alors la valeur provenant de boolean, double, integer ou string sera utilisée. Dans ce cas, il est attendu qu'une seule de {boolean, double, integer, or string} soit spécifiée. |
| [GetName](./getname/) | Le nom du paramètre. |
| [SetName](./setname/) | Le nom du paramètre. |
| [GetCellReference](./getcellreference/) | Référence de cellule indiquant quelle valeur de cellule utiliser pour le paramètre de requête. Utilisée uniquement lorsque parameterType est cell. |
| [SetCellReference](./setcellreference/) | Référence de cellule indiquant quelle valeur de cellule utiliser pour le paramètre de requête. Utilisée uniquement lorsque parameterType est cell. |
| [GetValue](./getvalue/) | Non-integer numeric value,Integer value,String value or Boolean value à utiliser comme paramètre de requête. Utilisée uniquement lorsque parameterType est value. |
| [SetValue](./setvalue/) | Non-integer numeric value,Integer value,String value or Boolean value à utiliser comme paramètre de requête. Utilisée uniquement lorsque parameterType est value. |
