---
title: "فئة Format3D"
linktitle: "Format3D"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "Format3D فئة. تغلف الكائن الذي يمثل format3d في Go."
type: docs
weight: 200
url: /ar/go-cpp/format3d/
---

## Format3D class

تحدد هذه الفئة خصائص الشكل ثلاثي الأبعاد لعنصر مخطط أو شكل.

```go

type Format3D struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetTopBevel](./gettopbevel/) | يحصل على كائن Bevel الذي يحتوي على الخصائص المرتبطة بتعريف الحافة على الوجه العلوي أو الأمامي للشكل. |
| [HasTopBevelData](./hastopbeveldata/) | يشير إلى ما إذا كان الشكل يحتوي على بيانات الحافة العلوية. |
| [GetSurfaceMaterialType](./getsurfacematerialtype/) | يحصل ويضبط نوع المادة الذي يُدمج مع خصائص الإضاءة لإعطاء المظهر والشعور النهائي للشكل. القيمة الافتراضية هي PresetMaterialType.WarmMatte. |
| [SetSurfaceMaterialType](./setsurfacematerialtype/) | يحصل ويضبط نوع المادة الذي يُدمج مع خصائص الإضاءة لإعطاء المظهر والشعور النهائي للشكل. القيمة الافتراضية هي PresetMaterialType.WarmMatte. |
| [GetSurfaceLightingType](./getsurfacelightingtype/) | يحصل ويضبط نوع الإضاءة الذي سيُطبق على مشهد الشكل. القيمة الافتراضية هي LightRigType.ThreePoint. |
| [SetSurfaceLightingType](./setsurfacelightingtype/) | يحصل ويضبط نوع الإضاءة الذي سيُطبق على مشهد الشكل. القيمة الافتراضية هي LightRigType.ThreePoint. |
| [GetLightingAngle](./getlightingangle/) | يسترجع ويعيّن زاوية الإضاءة. النطاق من 0 إلى 359.9 درجة. |
| [SetLightingAngle](./setlightingangle/) | يسترجع ويعيّن زاوية الإضاءة. النطاق من 0 إلى 359.9 درجة. |
