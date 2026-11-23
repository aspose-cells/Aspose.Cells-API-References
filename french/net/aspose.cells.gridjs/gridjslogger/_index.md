---
title: "Classe GridJsLogger"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.GridJs.GridJsLogger. Fournit un système de journalisation léger pour le serveur GridJs. Prend en charge la sortie console et fichier avec des niveaux de journalisation configurables. Le niveau par défaut est None. Dans une version DEBUG, le niveau par défaut est Debug qui affiche tous les messages. Prend en charge la rotation des fichiers de journal par jour/semaine/mois."
type: docs
url: /fr/net/aspose.cells.gridjs/gridjslogger/
---
## GridJsLogger class

Fournit un système de journalisation léger pour le serveur GridJs. Prend en charge la sortie console et fichier avec des niveaux de journalisation configurables. Le niveau par défaut est Aucun. Dans une version DEBUG, le niveau par défaut est Debug (affiche tous les messages). Prend en charge la rotation des fichiers journaux par jour/semaine/mois.

```csharp
public static class GridJsLogger
```

## Propriétés

| Nom | Description |
| --- | --- |
| static [EnableConsoleOutput](../../aspose.cells.gridjs/gridjslogger/enableconsoleoutput/) { get; set; } | Obtient ou définit si les messages de journal doivent être affichés dans la console. La valeur par défaut est false. |
| static [EnableFileOutput](../../aspose.cells.gridjs/gridjslogger/enablefileoutput/) { get; set; } | Obtient ou définit si les messages de journal doivent être écrits dans un fichier. La valeur par défaut est false. Vous devez appeler [`SetLogFile`](./setlogfile/) ou [`SetLogDirectory`](./setlogdirectory/) avant d'activer. |
| static [Level](../../aspose.cells.gridjs/gridjslogger/level/) { get; set; } | Obtient ou définit le niveau de journal minimum. Les messages en dessous de ce niveau seront ignorés. La valeur par défaut est None. |
| static [LogFilePath](../../aspose.cells.gridjs/gridjslogger/logfilepath/) { get; } | Obtient le chemin du fichier de journal actuel, ou null s'il n'est pas défini. |
| static [MaxFileSize](../../aspose.cells.gridjs/gridjslogger/maxfilesize/) { get; set; } | Obtient ou définit la taille maximale (en octets) d'un fichier de journal unique avant la rotation. Effectif uniquement lorsque la rotation est activée. 0 signifie aucune limite de taille. La valeur par défaut est 0. |

## Méthodes

| Nom | Description |
| --- | --- |
| static [CloseLogFile](../../aspose.cells.gridjs/gridjslogger/closelogfile/)() | Ferme l'écrivain du fichier de journal et désactive la sortie vers le fichier. |
| static [Debug](../../aspose.cells.gridjs/gridjslogger/debug/)(string) | Enregistre un message de niveau debug. |
| static [Error](../../aspose.cells.gridjs/gridjslogger/error/)(string) | Enregistre un message de niveau erreur. |
| static [Info](../../aspose.cells.gridjs/gridjslogger/info/)(string) | Enregistre un message de niveau info. |
| static [Log](../../aspose.cells.gridjs/gridjslogger/log/)(GridJsLogLevel, string) | Enregistre un message au niveau spécifié. |
| static [SetLogDirectory](../../aspose.cells.gridjs/gridjslogger/setlogdirectory/#setlogdirectory)(string) | Définit le répertoire de journal avec une stratégie de rotation quotidienne des fichiers et active la sortie vers le fichier. Les fichiers de journal seront nommés ainsi : gridjs_{period}.log |
| static [SetLogDirectory](../../aspose.cells.gridjs/gridjslogger/setlogdirectory/#setlogdirectory_1)(string, GridJsLogRolling) | Définit le répertoire de journal avec une stratégie de rotation des fichiers et active la sortie vers le fichier. Les fichiers de journal seront nommés ainsi : gridjs_{period}.log |
| static [SetLogDirectory](../../aspose.cells.gridjs/gridjslogger/setlogdirectory/#setlogdirectory_2)(string, GridJsLogRolling, string) | Définit le répertoire de journal avec une stratégie de rotation des fichiers et active la sortie vers le fichier. Les fichiers de journal seront nommés ainsi : {prefix}_{period}.log Exemples : gridjs_2026-07-27.log (quotidien), gridjs_2026-W30.log (hebdomadaire), gridjs_2026-07.log (mensuel) |
| static [SetLogFile](../../aspose.cells.gridjs/gridjslogger/setlogfile/#setlogfile)(string) | Définit le chemin du fichier de journal et active la sortie vers le fichier (mode fichier unique, sans rotation). Ajoute au fichier existant. |
| static [SetLogFile](../../aspose.cells.gridjs/gridjslogger/setlogfile/#setlogfile_1)(string, bool) | Définit le chemin du fichier de journal et active la sortie vers le fichier (mode fichier unique, sans rotation). Ajoute au fichier existant. |
| static [Warn](../../aspose.cells.gridjs/gridjslogger/warn/)(string) | Enregistre un message de niveau avertissement. |

### Voir aussi

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


