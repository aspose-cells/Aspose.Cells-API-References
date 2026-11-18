---
title: "Format3D-klass"
linktitle: "Format3D"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "Format3D-klass. Inkapslar objektet som representerar format3d i Go."
type: docs
weight: 200
url: /sv/go-cpp/format3d/
---

## Format3D class

Denna klass specificerar 3D‑formegenskaper för ett diagramelement eller en form.

```go

type Format3D struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetTopBevel](./gettopbevel/) | Hämtar Bevel-objektet som innehåller egenskaperna för att definiera en fasett på den övre eller främre ytan av en form. |
| [HasTopBevelData](./hastopbeveldata/) | Indikerar om formen har top-fasettdata. |
| [GetSurfaceMaterialType](./getsurfacematerialtype/) | Hämtar och anger materialtypen som kombineras med ljusegenskaperna för att ge formen dess slutgiltiga utseende och känsla. Standardvärdet är PresetMaterialType.WarmMatte. |
| [SetSurfaceMaterialType](./setsurfacematerialtype/) | Hämtar och anger materialtypen som kombineras med ljusegenskaperna för att ge formen dess slutgiltiga utseende och känsla. Standardvärdet är PresetMaterialType.WarmMatte. |
| [GetSurfaceLightingType](./getsurfacelightingtype/) | Hämtar och anger ljustypen som ska tillämpas på formens scen. Standardvärdet är LightRigType.ThreePoint. |
| [SetSurfaceLightingType](./setsurfacelightingtype/) | Hämtar och anger ljustypen som ska tillämpas på formens scen. Standardvärdet är LightRigType.ThreePoint. |
| [GetLightingAngle](./getlightingangle/) | Hämtar och anger belysningsvinkeln. Intervall från 0 till 359,9 grader. |
| [SetLightingAngle](./setlightingangle/) | Hämtar och anger belysningsvinkeln. Intervall från 0 till 359,9 grader. |
