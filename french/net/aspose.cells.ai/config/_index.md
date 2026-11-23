---
title: "Classe Config"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.AI.Config. Représente tous les paramètres pour Cells AI"
type: docs
url: /fr/net/aspose.cells.ai/config/
---
## Config class

Représente tous les paramètres pour Cells AI

```csharp
public class Config
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [Config](config/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| static [Model](../../aspose.cells.ai/config/model/) { get; set; } | Le modèle IA à utiliser |

## Champs

| Nom | Description |
| --- | --- |
| static [ContentChunkSize](../../aspose.cells.ai/config/contentchunksize/) | La taille du fragment de contenu dans la liste de messages pour l'IA par requête |
| static [InitialFailRetryDelay](../../aspose.cells.ai/config/initialfailretrydelay/) | Le temps de délai initial (ms) pour démarrer une nouvelle requête après un appel échoué |
| static [Locale](../../aspose.cells.ai/config/locale/) | La langue préférée pour le paramètre régional de l'utilisateur "ar", pour : "Arabic (العربية)" "bg", for: "Bulgarian (Български)" "ca", for: "Catalan (Català)" "cs", for: "Czech (Čeština)" "da", for: "Danish (Dansk)" "de", for: "German (Deutsch)" "el", for: "Greek (Ελληνικά)" "en", for: "English (English)" "es", for: "Spanish (Español)" "fa", for: "Persian (فارسی)" "fr", for: "French (Français)" "he", for: "Hebrew (עִברִית)" "hi", for: "Hindi (हिन्दी)" "hr", for: "Croatian (Hrvatski)" "hu", for: "Hungarian (Magyar)" "id", for: "Indonesian (Indonesia)" "it", for: "Italian (Italiano)" "ja", for: "Japanese (日本語)" "ka", for: "Georgian (ქართული)" "ko", for: "Korean (한국어)" "lt", for: "Lithuanian (Lietuvis)" "ms", for: "Malay (Bahasa Melayu)" "nl", for: "Dutch (Nederlands)" "pl", for: "Polish (Polskie)" "pt", for: "Portuguese (Português)" "ro", for: "Romanian (Română)" "ru", for: "Russian (Русский)" "sk", for: "Slovak (Slovák)" "th", for: "Thai (ภาษาไทย)" "tr", for: "Turkish (Türk)" "uk", for: "Ukrainian (Український)" "vi", for: "Vietnamese (Tiếng Việt)" "zh", for: "Simplified Chinese (简体中文)" "zh-hant", for: "Traditional Chinese (繁體中文)" |
| static [LogDirectory](../../aspose.cells.ai/config/logdirectory/) | Le répertoire du fichier journal |
| static [LogLevel](../../aspose.cells.ai/config/loglevel/) | s'il faut ajouter le journal |
| static [MaxRetryTimes](../../aspose.cells.ai/config/maxretrytimes/) | Le nombre maximal de tentatives de récupération d'une réponse de l'IA, si échec, démarrera une nouvelle requête. |
| static [MaxTokens](../../aspose.cells.ai/config/maxtokens/) | Le nombre maximal de jetons pour l'IA par requête |
| static [Temperature](../../aspose.cells.ai/config/temperature/) | La température IA par défaut à utiliser, lorsque la température approche 0, les choix du modèle deviennent très déterministes, sélectionnant presque toujours la sortie avec la plus haute probabilité. Lorsque la température approche 1 ou plus, les sorties du modèle deviennent plus aléatoires et diversifiées. |
| static [TimeOutSeconds](../../aspose.cells.ai/config/timeoutseconds/) | Le délai d'expiration en secondes pour que l'IA réponde |

### Voir aussi

* namespace [Aspose.Cells.AI](../../aspose.cells.ai/)
* assembly [CellsAI](../../)


