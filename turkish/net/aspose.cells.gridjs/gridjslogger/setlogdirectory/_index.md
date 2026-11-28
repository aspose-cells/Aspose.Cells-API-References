---
title: "GridJsLogger.SetLogDirectory"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GridJsLogger yöntemi. Günlük dizinini günlük dönen dosya stratejisiyle ayarlar ve dosya çıkışını etkinleştirir. Günlük dosyaları gridjs_period.log olarak adlandırılacaktır"
type: docs
url: /tr/net/aspose.cells.gridjs/gridjslogger/setlogdirectory/
---
## SetLogDirectory(string) {#setlogdirectory}

Günlük dizinini günlük döndürme dosya stratejisiyle ayarlar ve dosya çıktısını etkinleştirir. Günlük dosyaları şu şekilde adlandırılır: gridjs_{period}.log

```csharp
public static void SetLogDirectory(string directory)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| directory | String | Günlük dosyalarını depolamak için dizin. |

### Ayrıca Bakınız

* class [GridJsLogger](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)

---

## SetLogDirectory(string, GridJsLogRolling) {#setlogdirectory_1}

Günlük dizinini döndürme dosya stratejisiyle ayarlar ve dosya çıktısını etkinleştirir. Günlük dosyaları şu şekilde adlandırılır: gridjs_{period}.log

```csharp
public static void SetLogDirectory(string directory, GridJsLogRolling rolling)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| directory | String | Günlük dosyalarını depolamak için dizin. |
| rolling | GridJsLogRolling | Dönen strateji (Günlük/Haftalık/Aylık). |

### Ayrıca Bakınız

* enum [GridJsLogRolling](../../gridjslogrolling/)
* class [GridJsLogger](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)

---

## SetLogDirectory(string, GridJsLogRolling, string) {#setlogdirectory_2}

Günlük dizinini döndürme dosya stratejisiyle ayarlar ve dosya çıktısını etkinleştirir. Günlük dosyaları şu şekilde adlandırılır: {prefix}_{period}.log Örnekler: gridjs_2026-07-27.log (Günlük), gridjs_2026-W30.log (Haftalık), gridjs_2026-07.log (Aylık)

```csharp
public static void SetLogDirectory(string directory, GridJsLogRolling rolling, string filePrefix)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| directory | String | Günlük dosyalarını depolamak için dizin. |
| rolling | GridJsLogRolling | Dönen strateji (Günlük/Haftalık/Aylık). |
| filePrefix | String | Dosya adı öneki. |

### Ayrıca Bakınız

* enum [GridJsLogRolling](../../gridjslogrolling/)
* class [GridJsLogger](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


