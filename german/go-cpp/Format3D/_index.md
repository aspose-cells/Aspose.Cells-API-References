---
title: "Format3D Klasse"
linktitle: "Format3D"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "Format3D Klasse. Kapselt das Objekt, das format3d in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/format3d/
---

## Format3D class

Diese Klasse gibt die 3D-Formeigenschaften für ein Diagrammelement oder eine Form an.

```go

type Format3D struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetTopBevel](./gettopbevel/) | Liefert das Bevel‑Objekt, das die Eigenschaften enthält, die mit der Definition einer Abschrägung an der oberen oder vorderen Fläche einer Form verbunden sind. |
| [HasTopBevelData](./hastopbeveldata/) | Gibt an, ob die Form obere Abschrägungsdaten hat. |
| [GetSurfaceMaterialType](./getsurfacematerialtype/) | Liest und setzt den Materialtyp, der mit den Lichteigenschaften kombiniert wird, um das endgültige Aussehen einer Form zu erzeugen. Standardwert ist PresetMaterialType.WarmMatte. |
| [SetSurfaceMaterialType](./setsurfacematerialtype/) | Liest und setzt den Materialtyp, der mit den Lichteigenschaften kombiniert wird, um das endgültige Aussehen einer Form zu erzeugen. Standardwert ist PresetMaterialType.WarmMatte. |
| [GetSurfaceLightingType](./getsurfacelightingtype/) | Liest und setzt den Beleuchtungstyp, der auf die Szene der Form angewendet wird. Standardwert ist LightRigType.ThreePoint. |
| [SetSurfaceLightingType](./setsurfacelightingtype/) | Liest und setzt den Beleuchtungstyp, der auf die Szene der Form angewendet wird. Standardwert ist LightRigType.ThreePoint. |
| [GetLightingAngle](./getlightingangle/) | Liest und setzt den Beleuchtungswinkel. Bereich von 0 bis 359,9 Grad. |
| [SetLightingAngle](./setlightingangle/) | Liest und setzt den Beleuchtungswinkel. Bereich von 0 bis 359,9 Grad. |
