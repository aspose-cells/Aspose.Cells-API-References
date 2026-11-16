---
title: "GetCheckExcelRestriction Méthode"
linktitle: "GetCheckExcelRestriction"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "GetCheckExcelRestriction méthode. Encapsule la fonction qui représente getcheckexcelrestriction en Go."
type: docs
weight: 200
url: /fr/go-cpp/xmlloadoptions/getcheckexcelrestriction/
---

## GetCheckExcelRestriction function

Indique si la restriction du fichier excel est vérifiée lorsque l'utilisateur modifie des objets liés aux cellules. Par exemple, excel n'autorise pas la saisie d'une chaîne de caractères supérieure à 32 K. Lorsque vous saisissez une valeur supérieure à 32 K, par exemple avec Cell.PutValue(string), si cette propriété est vraie, vous obtiendrez une Exception. Si cette propriété est fausse, nous accepterons votre chaîne saisie comme valeur de la cellule afin que vous puissiez ensuite exporter la chaîne complète vers d'autres formats de fichier tels que CSV. Cependant, si vous avez défini une valeur qui n'est pas valide pour le format de fichier excel, vous ne devez pas enregistrer le workbook au format excel ultérieurement. Sinon, il peut y avoir des erreurs inattendues dans le fichier excel généré.

```go

func (instance *XmlLoadOptions) GetCheckExcelRestriction()  (bool,  error) 

```

## Remarques


## Voir aussi

* Class [XmlLoadOptions](../)
* Library [Aspose.Cells for Go](../../)
