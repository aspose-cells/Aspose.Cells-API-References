---
title: "Format3D Class"
linktitle: "Format3D"
articleTitle: "Format3D"
second_title: "Aspose.Cells for Python via Java"
description: "This class specifies the 3D shape properties for a chart element or shape."
type: docs
weight: 2530
url: /python-java/asposecells.api/format3d/
---

## Format3D class

This class specifies the 3D shape properties for a chart element or shape.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [TopBevel](#topbevel) | Bevel | Gets the Bevel object that holds the properties associated with defining a bevel on the top or front face of a shape. |
| [SurfaceMaterialType](#surfacematerialtype) | int | Gets and sets the material type which is combined with the lighting properties to give the final look and feel of a shap |
| [SurfaceLightingType](#surfacelightingtype) | int | Gets and sets the lighting type which is to be applied to the scene of the shape. Default value is LightRigType.ThreePoi |
| [LightingAngle](#lightingangle) | float | Gets and sets the lighting angle. Range from 0 to 359.9 degrees. |

## Methods

| Name | Description |
| --- | --- |
| [hasTopBevelData](#hastopbeveldata) | Indicates if the shape has top bevel data. |

### Format3D.TopBevel property {#topbevel}

Gets the Bevel object that holds the properties associated with defining a bevel on the top or front face of a shape.

**Type:** Bevel

### Format3D.SurfaceMaterialType property {#surfacematerialtype}

Gets and sets the material type which is combined with the lighting properties to give the final look and feel of a shape. Default value is PresetMaterialType.WarmMatte. The value of the property is PresetMaterialType integer constant.

**Type:** int

### Format3D.SurfaceLightingType property {#surfacelightingtype}

Gets and sets the lighting type which is to be applied to the scene of the shape. Default value is LightRigType.ThreePoint. The value of the property is LightRigType integer constant.

**Type:** int

### Format3D.LightingAngle property {#lightingangle}

Gets and sets the lighting angle. Range from 0 to 359.9 degrees.

**Type:** float

### hasTopBevelData() {#hastopbeveldata}

Indicates if the shape has top bevel data.
