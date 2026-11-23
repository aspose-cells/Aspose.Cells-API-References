---
title: "SpreadsheetConverter.Process"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SpreadsheetConverter. Convertit le fichier de modèle donné entre les formats de fichiers de feuille de calcul"
type: docs
url: /fr/net/aspose.cells.lowcode/spreadsheetconverter/process/
---
## Process(string, string) {#process_1}

Convertit le fichier modèle fourni entre différents formats de fichiers tableur.

```csharp
public static void Process(string templateFile, string resultFile)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| templateFile | String | Le fichier modèle à convertir |
| resultFile | String | Le fichier résultant |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetConverterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            SpreadsheetConverter.Process("file1.xlsx", "SpreadsheetConverterMethodProcessWithStringStringDemo.xlsb");
        }
    }
}
```

### Voir aussi

* class [SpreadsheetConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

Convertit entre différents formats de fichiers tableur.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Options d'entrée et de chargement |
| saveOptions | LowCodeSaveOptions | Options de sortie et d'enregistrement |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
    {
        public static void Run()
        {
            // Créer des options de chargement avec le fichier d'entrée
            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            loadOptions.InputFile = "file1.xlsx";

            // Créer des options d'enregistrement avec le fichier de sortie
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
            saveOptions.OutputFile = "SpreadsheetConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo.xlsx";

            // Exécuter la conversion
            SpreadsheetConverter.Process(loadOptions, saveOptions);
        }
    }
}
```

### Voir aussi

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [SpreadsheetConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


