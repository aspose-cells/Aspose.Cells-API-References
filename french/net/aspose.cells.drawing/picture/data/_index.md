---
title: Data
second_title: Référence de l'API Aspose.Cells pour .NET
description: Obtient les données de limage.
type: docs
weight: 30
url: /fr/net/aspose.cells.drawing/picture/data/
---
## Picture.Data property

Obtient les données de l'image.

```csharp
public byte[] Data { get; set; }
```

### Exemples

```csharp

[C#]
//Instanciation d'un objet Workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
//insérer la première image
int imgIndex1 = worksheet.Pictures.Add(1, 1, "example1.png");
// Récupère l'objet image inséré
Picture pic1 = worksheet.Pictures[imgIndex1];
//insérer une deuxième image
int imgIndex2 = worksheet.Pictures.Add(1, 9, "example2.jpeg");
// Récupère l'objet image inséré
Picture pic2 = worksheet.Pictures[imgIndex2];
//Assigne les données en octets de la première image à la deuxième image
pic2.Data = pic1.Data;
// Enregistrez le fichier excel.
workbook.Save("result.xlsx");
```

### Voir également

* class [Picture](../../picture)
* espace de noms [Aspose.Cells.Drawing](../../picture)
* Assemblée [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
