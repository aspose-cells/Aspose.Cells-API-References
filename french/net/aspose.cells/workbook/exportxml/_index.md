---
title: ExportXml
second_title: Référence de l'API Aspose.Cells pour .NET
description: Exporter les données XML liées par le mappage XML spécifié.
type: docs
weight: 400
url: /fr/net/aspose.cells/workbook/exportxml/
---
## ExportXml(string, string) {#exportxml_1}

Exporter les données XML liées par le mappage XML spécifié.

```csharp
public void ExportXml(string mapName, string path)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| mapName | String | nom de la carte XML à exporter |
| path | String | le chemin d'exportation |

### Exemples

Le code suivant a exporté les données liées par le premier XmlMap.

```csharp
Workbook wb = new Workbook("Book1.xlsx");

//Assurez-vous que le fichier xlsx source contient un XmlMap.
XmlMap xmlMap = wb.Worksheets.XmlMaps[0];

wb.ExportXml(xmlMap.Name, "output.xml");
```

### Voir également

* class [Workbook](../../workbook)
* espace de noms [Aspose.Cells](../../workbook)
* Assemblée [Aspose.Cells](../../../)

---

## ExportXml(string, Stream) {#exportxml}

Exporter les données XML.

```csharp
public void ExportXml(string mapName, Stream stream)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| mapName | String | nom de la carte XML à exporter |
| stream | Stream | le flux d'exportation |

### Voir également

* class [Workbook](../../workbook)
* espace de noms [Aspose.Cells](../../workbook)
* Assemblée [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
