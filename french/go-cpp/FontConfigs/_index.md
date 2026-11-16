---
title: "Classe FontConfigs"
linktitle: "FontConfigs"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe FontConfigs. Encapsule l'objet qui représente les fontconfigs en Go."
type: docs
weight: 200
url: /fr/go-cpp/fontconfigs/
---

## FontConfigs class

Spécifie les paramètres de police

```go

type FontConfigs struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewFontConfigs](./newfontconfigs/) | Constructeur par défaut. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [FontConfigs_IsFontAvailable](./fontconfigs_isfontavailable/) | Indique si la police est disponible. |
| [FontConfigs_GetFontFileDataInfo](./fontconfigs_getfontfiledatainfo/) | Obtenez les informations de données du fichier de police. |
| [FontConfigs_GetDefaultFontName](./fontconfigs_getdefaultfontname/) | Obtient ou définit le nom de police par défaut. |
| [FontConfigs_SetDefaultFontName](./fontconfigs_setdefaultfontname/) | Obtient ou définit le nom de police par défaut. |
| [FontConfigs_GetPreferSystemFontSubstitutes](./fontconfigs_getprefersystemfontsubstitutes/) | Indique s'il faut utiliser d'abord les substituts de police système ou non lorsqu'une police n'est pas présentée et que le substitut de cette police n'est pas défini. Par exemple, sous Ubuntu, la police "Arial" est généralement remplacée par "Liberation Sans". La valeur par défaut est false. |
| [FontConfigs_SetPreferSystemFontSubstitutes](./fontconfigs_setprefersystemfontsubstitutes/) | Indique s'il faut utiliser d'abord les substituts de police système ou non lorsqu'une police n'est pas présentée et que le substitut de cette police n'est pas défini. Par exemple, sous Ubuntu, la police "Arial" est généralement remplacée par "Liberation Sans". La valeur par défaut est false. |
| [FontConfigs_SetFontSubstitutes](./fontconfigs_setfontsubstitutes/) | Noms de substituts de police pour le nom de police original donné. |
| [FontConfigs_GetFontSubstitutes](./fontconfigs_getfontsubstitutes/) | Renvoie un tableau contenant les noms de substituts de police à utiliser si la police originale n'est pas présente. |
| [FontConfigs_SetFontFolder](./fontconfigs_setfontfolder/) | Définit le dossier des polices |
| [FontConfigs_SetFontFolders](./fontconfigs_setfontfolders/) | Définit le dossier des polices |
| [FontConfigs_SetFontSources](./fontconfigs_setfontsources/) | Définit les sources de police. |
| [FontConfigs_GetFontSources](./fontconfigs_getfontsources/) | Obtient une copie du tableau qui contient la liste des sources |
