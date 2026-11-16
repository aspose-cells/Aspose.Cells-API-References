---
title: "Format3D 类"
linktitle: "Format3D"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "Format3D 类。封装表示 Go 中 format3d 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/format3d/
---

## Format3D class

此类指定图表元素或形状的 3D 形状属性。

```go

type Format3D struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetTopBevel](./gettopbevel/) | 获取 Bevel 对象，该对象保存与在形状的顶部或前面定义斜角相关的属性。 |
| [HasTopBevelData](./hastopbeveldata/) | 指示形状是否具有顶部斜角数据。 |
| [GetSurfaceMaterialType](./getsurfacematerialtype/) | 获取和设置材质类型，该类型与光照属性相结合，以提供形状的最终外观和感觉。默认值为 PresetMaterialType.WarmMatte。 |
| [SetSurfaceMaterialType](./setsurfacematerialtype/) | 获取和设置材质类型，该类型与光照属性相结合，以提供形状的最终外观和感觉。默认值为 PresetMaterialType.WarmMatte。 |
| [GetSurfaceLightingType](./getsurfacelightingtype/) | 获取和设置将应用于形状场景的光照类型。默认值为 LightRigType.ThreePoint。 |
| [SetSurfaceLightingType](./setsurfacelightingtype/) | 获取和设置将应用于形状场景的光照类型。默认值为 LightRigType.ThreePoint。 |
| [GetLightingAngle](./getlightingangle/) | 获取并设置光照角度。范围从 0 到 359.9 度。 |
| [SetLightingAngle](./setlightingangle/) | 获取并设置光照角度。范围从 0 到 359.9 度。 |
