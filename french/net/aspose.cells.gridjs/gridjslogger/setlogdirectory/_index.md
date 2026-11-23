---
title: "GridJsLogger.SetLogDirectory"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "GridJsLogger méthode. Définit le répertoire de journal avec une stratégie de rotation quotidienne des fichiers et active la sortie vers un fichier. Les fichiers de journal seront nommés comme gridjs_period.log"
type: docs
url: /fr/net/aspose.cells.gridjs/gridjslogger/setlogdirectory/
---
## SetLogDirectory(string) {#setlogdirectory}

Définit le répertoire de journal avec une stratégie de rotation quotidienne des fichiers et active la sortie vers le fichier. Les fichiers de journal seront nommés ainsi : gridjs_{period}.log

```csharp
public static void SetLogDirectory(string directory)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| répertoire | String | Le répertoire où stocker les fichiers de journal. |

### Voir aussi

* class [GridJsLogger](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)

---

## SetLogDirectory(string, GridJsLogRolling) {#setlogdirectory_1}

Définit le répertoire de journal avec une stratégie de rotation des fichiers et active la sortie vers le fichier. Les fichiers de journal seront nommés ainsi : gridjs_{period}.log

```csharp
public static void SetLogDirectory(string directory, GridJsLogRolling rolling)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| répertoire | String | Le répertoire où stocker les fichiers de journal. |
| rotation | GridJsLogRolling | La stratégie de rotation (Daily/Weekly/Monthly). |

### Voir aussi

* enum [GridJsLogRolling](../../gridjslogrolling/)
* class [GridJsLogger](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)

---

## SetLogDirectory(string, GridJsLogRolling, string) {#setlogdirectory_2}

Définit le répertoire de journal avec une stratégie de rotation des fichiers et active la sortie vers le fichier. Les fichiers de journal seront nommés ainsi : {prefix}_{period}.log Exemples : gridjs_2026-07-27.log (quotidien), gridjs_2026-W30.log (hebdomadaire), gridjs_2026-07.log (mensuel)

```csharp
public static void SetLogDirectory(string directory, GridJsLogRolling rolling, string filePrefix)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| répertoire | String | Le répertoire où stocker les fichiers de journal. |
| rotation | GridJsLogRolling | La stratégie de rotation (Daily/Weekly/Monthly). |
| filePrefix | String | Le préfixe du nom de fichier. |

### Voir aussi

* enum [GridJsLogRolling](../../gridjslogrolling/)
* class [GridJsLogger](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


