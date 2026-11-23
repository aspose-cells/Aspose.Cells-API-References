---
title: "SpreadsheetMerger.Process"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SpreadsheetMerger. Fusionner les fichiers de modèle fournis"
type: docs
url: /fr/net/aspose.cells.lowcode/spreadsheetmerger/process/
---
## Process(string[], string) {#process_1}

Fusionner les fichiers modèle fournis.

```csharp
public static void Process(string[] templateFiles, string resultFile)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| templateFiles | String[] | Les fichiers de modèle à fusionner |
| resultFile | String | Le fichier résultant |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetMergerMethodProcessWithStringArrayStringDemo
    {
        public static void Run()
        {
            // Créer des fichiers de modèle d'exemple
            CreateTemplateFile("template1.xlsx", "Data from Template 1");
            CreateTemplateFile("template2.xlsx", "Data from Template 2");

            string[] templateFiles = { "template1.xlsx", "template2.xlsx" };
            string resultFile = "merged_output.xlsx";

            try
            {
                SpreadsheetMerger.Process(templateFiles, resultFile);

                Console.WriteLine($"Process method merged {templateFiles.Length} files into {resultFile}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Process method: {ex.Message}");
            }
        }

        private static void CreateTemplateFile(string fileName, string cellValue)
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue(cellValue);
            workbook.Save(fileName);
        }
    }
}
```

### Voir aussi

* class [SpreadsheetMerger](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeMergeOptions) {#process}

Fusionne plusieurs fichiers modèle en un seul.

```csharp
public static void Process(LowCodeMergeOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| options | LowCodeMergeOptions | Options pour fusionner les fichiers |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetMergerMethodProcessWithLowCodeMergeOptDemo
    {
        public static void Run()
        {
            // Préparer deux fichiers de modèle simples qui seront fusionnés.
            CreateTemplateFile("TemplateA.xlsx", "Data from Template A");
            CreateTemplateFile("TemplateB.xlsx", "Data from Template B");

            try
            {
                // Créer une instance de la classe d'options.
                // La classe LowCodeMergeOptions fait partie de Aspose.Cells.LowCode.
                // Pour cette démonstration, nous utilisons le constructeur par défaut.
                LowCodeMergeOptions options = new LowCodeMergeOptions();

                // Appelez la méthode Process qui accepte LowCodeMergeOptions.
                SpreadsheetMerger.Process(options);

                Console.WriteLine("Process method invoked successfully with LowCodeMergeOptions.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Process: {ex.Message}");
            }
        }

        private static void CreateTemplateFile(string fileName, string cellValue)
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue(cellValue);
            workbook.Save(fileName);
        }
    }
}
```

### Voir aussi

* class [LowCodeMergeOptions](../../lowcodemergeoptions/)
* class [SpreadsheetMerger](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


