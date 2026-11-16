---
title: "Format3D Classe"
linktitle: "Format3D"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe Format3D. Encapsule l'objet qui représente format3d en Go."
type: docs
weight: 200
url: /fr/go-cpp/format3d/
---

## Format3D class

Cette classe spécifie les propriétés de forme 3D pour un élément de graphique ou une forme.

```go

type Format3D struct  {
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
| [GetTopBevel](./gettopbevel/) | Obtient l'objet Bevel qui contient les propriétés associées à la définition d'un biseau sur la face supérieure ou avant d'une forme. |
| [HasTopBevelData](./hastopbeveldata/) | Indique si la forme possède des données de biseau supérieur. |
| [GetSurfaceMaterialType](./getsurfacematerialtype/) | Obtient et définit le type de matériau qui est combiné aux propriétés d'éclairage pour donner l'apparence finale d'une forme. La valeur par défaut est PresetMaterialType.WarmMatte. |
| [SetSurfaceMaterialType](./setsurfacematerialtype/) | Obtient et définit le type de matériau qui est combiné aux propriétés d'éclairage pour donner l'apparence finale d'une forme. La valeur par défaut est PresetMaterialType.WarmMatte. |
| [GetSurfaceLightingType](./getsurfacelightingtype/) | Obtient et définit le type d'éclairage qui doit être appliqué à la scène de la forme. La valeur par défaut est LightRigType.ThreePoint. |
| [SetSurfaceLightingType](./setsurfacelightingtype/) | Obtient et définit le type d'éclairage qui doit être appliqué à la scène de la forme. La valeur par défaut est LightRigType.ThreePoint. |
| [GetLightingAngle](./getlightingangle/) | Obtient et définit l'angle d'éclairage. Plage de 0 à 359,9 degrés. |
| [SetLightingAngle](./setlightingangle/) | Obtient et définit l'angle d'éclairage. Plage de 0 à 359,9 degrés. |
