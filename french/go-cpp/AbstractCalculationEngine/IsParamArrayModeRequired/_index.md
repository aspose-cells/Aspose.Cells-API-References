---
title: "IsParamArrayModeRequired Méthode"
linktitle: "IsParamArrayModeRequired"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "IsParamArrayModeRequired méthode. Encapsule la fonction qui représente isparamarraymoderequired en Go."
type: docs
weight: 200
url: /fr/go-cpp/abstractcalculationengine/isparamarraymoderequired/
---

## IsParamArrayModeRequired function

Indique si ce moteur a besoin que le paramètre soit calculé en mode tableau. La valeur par défaut est false. Si CalculationData.GetParamValueInArrayMode(int, int, int) est requis lors du calcul de customfunctions et que l’utilisateur n’a pas mis à jour la définition pour ceux‑ci (par Workbook.UpdateCustomFunctionDefinition(CustomFunctionDefinition)), cette propriété doit être définie sur true.

```go

func (instance *AbstractCalculationEngine) IsParamArrayModeRequired()  (bool,  error) 

```

## Remarques


## Voir aussi

* Class [AbstractCalculationEngine](../)
* Library [Aspose.Cells for Go](../../)
