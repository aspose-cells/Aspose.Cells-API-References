---
title: "GetSecondCommand Méthode"
linktitle: "GetSecondCommand"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "GetSecondCommand méthode. Encapsule la fonction qui représente getsecondcommand en Go."
type: docs
weight: 200
url: /fr/go-cpp/dbconnection/getsecondcommand/
---

## GetSecondCommand function

Spécifie une deuxième chaîne de texte de commande qui est conservée lorsque les champs de page basés sur le serveur de PivotTable sont utilisés. Pour les connexions ODBC, serverCommand est généralement une requête plus large que command (aucune clause WHERE n'est présente dans la première). En se basant sur ces 2 commandes (Command et ServerCommand), l'interface utilisateur des paramètres peut être remplie et des requêtes paramétrées peuvent être construites.

```go

func (instance *DBConnection) GetSecondCommand()  (string,  error) 

```

## Remarques


## Voir aussi

* Class [DBConnection](../)
* Library [Aspose.Cells for Go](../../)
