---
title: "Workbook.Copy"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Workbook. Copie un autre objet Workbook"
type: docs
url: /fr/net/aspose.cells/workbook/copy/
---
## Copy(Workbook, CopyOptions) {#copy_1}

Copie un autre objet Workbook.

```csharp
public void Copy(Workbook source, CopyOptions copyOptions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| source | Classeur | Objet Workbook source. |
| copyOptions | CopyOptions | Les options de copie d'un autre Workbook. |

### Remarques

Il est très simple de cloner un fichier Excel.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCopyWithWorkbookCopyOptionsDemo
    {
        public static void Run()
        {
            // Classeur source avec macros
            Workbook sourceWorkbook = new Workbook("source_with_macros.xlsm");
            
            // Classeur de destination (vide ou existant)
            Workbook destWorkbook = new Workbook();
            
            // Configurer les options de copie pour conserver les macros
            CopyOptions options = new CopyOptions();
            options.KeepMacros = true;
            
            // Copier le contenu du classeur source vers le classeur de destination
            sourceWorkbook.Copy(destWorkbook, options);
            
            // Enregistrer le résultat
            destWorkbook.Save("output_with_macros.xlsm");
        }
    }
}
```

### Voir aussi

* class [CopyOptions](../../copyoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Copy(Workbook) {#copy}

Copie les données d'un objet Workbook source.

```csharp
public void Copy(Workbook source)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| source | Classeur | Objet Workbook source. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCopyWithWorkbookDemo
    {
        public static void Run()
        {
            // Chemins des fichiers source et de sortie
            string sourceFile = "source.xlsx";
            string outputFile = "output.xlsx";

            // Charger le classeur source
            Workbook sourceWorkbook = new Workbook(sourceFile);

            // Créer un nouveau classeur et copier le contenu depuis la source
            Workbook destinationWorkbook = new Workbook();
            destinationWorkbook.Copy(sourceWorkbook);

            // Enregistrer le classeur copié
            destinationWorkbook.Save(outputFile);
            
            Console.WriteLine("Workbook copied successfully.");
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


