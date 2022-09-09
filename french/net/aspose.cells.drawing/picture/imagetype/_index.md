---
title: ImageType
second_title: Référence de l'API Aspose.Cells pour .NET
description: Obtient le format dimage de limage.
type: docs
weight: 60
url: /fr/net/aspose.cells.drawing/picture/imagetype/
---
## Picture.ImageType property

Obtient le format d'image de l'image.

```csharp
public ImageType ImageType { get; }
```

### Exemples

```csharp

[C#]
//Instanciation d'un objet Workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
//insérer la première image
int imgIndex1 = worksheet.Pictures.Add(1, 1, "1.png");
// Récupère l'objet image inséré
Picture pic1 = worksheet.Pictures[imgIndex1];
if(pic1.ImageType == Aspose.Cells.Drawing.ImageType.Png)
{
    //Le type de l'image est png.";
}
//insérer une deuxième image
int imgIndex2 = worksheet.Pictures.Add(1, 9, "2.jpeg");
// Récupère l'objet image inséré
Picture pic2 = worksheet.Pictures[imgIndex2];
if(pic2.ImageType == Aspose.Cells.Drawing.ImageType.Jpeg)
{
    //Le type de l'image est jpg.";
}
```

### Voir également

* enum [ImageType](../../imagetype)
* class [Picture](../../picture)
* espace de noms [Aspose.Cells.Drawing](../../picture)
* Assemblée [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->