---
title: "Format3D Sınıfı"
linktitle: "Format3D"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "Format3D sınıfı. Go'da format3d'yi temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/format3d/
---

## Format3D class

Bu sınıf, bir grafik öğesi veya şekil için 3B şekil özelliklerini belirtir.

```go

type Format3D struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetTopBevel](./gettopbevel/) | Şeklin üst veya ön yüzünde bir köşe tanımlamaya ilişkin özellikleri tutan Bevel nesnesini alır. |
| [HasTopBevelData](./hastopbeveldata/) | Şeklin üst köşe verisine sahip olup olmadığını gösterir. |
| [GetSurfaceMaterialType](./getsurfacematerialtype/) | Şeklin son görünüm ve hissini vermek için aydınlatma özellikleriyle birleştirilen malzeme türünü alır ve ayarlar. Varsayılan değer PresetMaterialType.WarmMatte'dir. |
| [SetSurfaceMaterialType](./setsurfacematerialtype/) | Şeklin son görünüm ve hissini vermek için aydınlatma özellikleriyle birleştirilen malzeme türünü alır ve ayarlar. Varsayılan değer PresetMaterialType.WarmMatte'dir. |
| [GetSurfaceLightingType](./getsurfacelightingtype/) | Şeklin sahnesine uygulanacak aydınlatma tipini alır ve ayarlar. Varsayılan değer LightRigType.ThreePoint'tir. |
| [SetSurfaceLightingType](./setsurfacelightingtype/) | Şeklin sahnesine uygulanacak aydınlatma tipini alır ve ayarlar. Varsayılan değer LightRigType.ThreePoint'tir. |
| [GetLightingAngle](./getlightingangle/) | Aydınlatma açısını alır ve ayarlar. Aralık 0 ile 359.9 derece arasında. |
| [SetLightingAngle](./setlightingangle/) | Aydınlatma açısını alır ve ayarlar. Aralık 0 ile 359.9 derece arasında. |
