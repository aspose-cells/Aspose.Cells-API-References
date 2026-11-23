---
title: "Worksheet.Copy"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Worksheet. Copie le contenu et les formats d’une autre feuille de calcul"
type: docs
url: /fr/net/aspose.cells/worksheet/copy/
---
## Copy(Worksheet) {#copy}

Copie le contenu et les formats d'une autre feuille de calcul.

```csharp
public void Copy(Worksheet sourceSheet)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sourceSheet | Feuille de calcul | Feuille source. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCopyWithWorksheetDemo
    {
        public static void Run()
        {
            // Créer un classeur source avec des données d'exemple
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            sourceSheet.Cells["A1"].PutValue("Source Worksheet");
            
            // Créer un classeur de destination
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // Copier la feuille source vers la feuille de destination
            destSheet.Copy(sourceSheet);
            
            // Enregistrer le résultat
            destWorkbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Copy(Worksheet, CopyOptions) {#copy_1}

Copie le contenu et les formats d'une autre feuille de calcul.

```csharp
public void Copy(Worksheet sourceSheet, CopyOptions copyOptions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sourceSheet | Feuille de calcul | Feuille source. |
| copyOptions | CopyOptions |  |

### Remarques

Vous pouvez copier des données d’une autre feuille de calcul dans le même fichier ou dans un autre fichier. Cependant, cette méthode ne prend pas en charge la copie d’objets graphiques, tels que les commentaires, les images et les graphiques.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCopyWithWorksheetCopyOptionsDemo
    {
        public static void Run()
        {
            // Créer le classeur source avec des données d'exemple
            Workbook srcWorkbook = new Workbook();
            Worksheet srcSheet = srcWorkbook.Worksheets[0];
            srcSheet.Name = "SourceSheet";
            srcSheet.Cells["A1"].PutValue("Source Data");

            // Créer le classeur de destination
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            destSheet.Name = "DestinationSheet";

            // Configurer les options de copie
            CopyOptions options = new CopyOptions();
            options.ReferToDestinationSheet = true;

            // Copier la feuille avec des options
            srcSheet.Copy(destSheet, options);

            // Vérifier l’opération de copie
            Console.WriteLine("Copied cell value: " + destSheet.Cells["A1"].StringValue);
            
            // Enregistrer le résultat
            destWorkbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [CopyOptions](../../copyoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


