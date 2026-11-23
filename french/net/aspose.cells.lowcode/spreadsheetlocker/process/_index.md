---
title: "SpreadsheetLocker.Process"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SpreadsheetLocker. Verrouille le fichier de feuille de calcul avec les paramètres spécifiés"
type: docs
url: /fr/net/aspose.cells.lowcode/spreadsheetlocker/process/
---
## Process(string, string, string, string) {#process_3}

Verrouille le fichier de feuille de calcul avec les paramètres spécifiés.

```csharp
public static void Process(string templateFile, string resultFile, string openPassword, 
    string writePassword)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| templateFile | String | Le fichier modèle à verrouiller |
| resultFile | String | Le fichier résultant |
| openPassword | String | Mot de passe pour le chiffrement du fichier |
| writePassword | String | Mot de passe pour la protection de la modification de la feuille de calcul |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class SpreadsheetLockerMethodProcessWithStringStringStringStringDemo
    {
        public static void Run()
        {           
            string templatePath = "template.xlsx";            
            // Préparer le chemin du fichier résultat
            string resultPath = "secured_spreadsheet.xlsx";

            try
            {
                // Exécuter la méthode Process avec des paramètres de chaîne directement en utilisant le type
                SpreadsheetLocker.Process(
                    templateFile: templatePath,
                    resultFile: resultPath,
                    openPassword: "Open@123",
                    writePassword: "Write@456"
                );

                Console.WriteLine($"Spreadsheet secured successfully. Saved to: {Path.GetFullPath(resultPath)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error securing spreadsheet: {ex.Message}");
            }
            finally
            {
                // Nettoyer le modèle temporaire
                if (File.Exists(templatePath))
                {
                    File.Delete(templatePath);
                }
            }
        }
    }
}
```

### Voir aussi

* class [SpreadsheetLocker](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions, string, string) {#process_1}

Verrouille le fichier de feuille de calcul avec les paramètres spécifiés.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, 
    string openPassword, string writePassword)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Options d'entrée et de chargement |
| saveOptions | LowCodeSaveOptions | Options de sortie et d'enregistrement |
| openPassword | String | Mot de passe pour le chiffrement du fichier |
| writePassword | String | Mot de passe pour la protection de la modification de la feuille de calcul |

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class SpreadsheetLockerMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
    {
        public static void Run()
        {
            
            // Traitez la feuille de calcul avec les mots de passe de verrouillage/déverrouillage
            SpreadsheetLocker.Process(
                new LowCodeLoadOptions() { InputFile = "input.xlsx" },
                new LowCodeSaveOptions() 
                { 
                    OutputFile = "output_locked.xlsx" 
                }, 
                "123456", 
                "234567");
        }
    }
}
```

### Voir aussi

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [SpreadsheetLocker](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions, string, string, string, ProtectionType) {#process_2}

Verrouille le fichier de feuille de calcul avec les paramètres spécifiés.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, 
    string openPassword, string writePassword, string workbookPassword, ProtectionType workbookType)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Options d'entrée et de chargement |
| saveOptions | LowCodeSaveOptions | Options de sortie et d'enregistrement |
| openPassword | String | Mot de passe pour le chiffrement du fichier |
| writePassword | String | Mot de passe pour la protection de la modification de la feuille de calcul |
| workbookPassword | String | Mot de passe pour la protection du classeur |
| workbookType | ProtectionType | Type de protection pour protéger le classeur |

### Voir aussi

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* enum [ProtectionType](../../../aspose.cells/protectiontype/)
* class [SpreadsheetLocker](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions, AbstractLowCodeProtectionProvider) {#process}

Verrouille le fichier de feuille de calcul avec les paramètres spécifiés.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, 
    AbstractLowCodeProtectionProvider provider)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Options d'entrée et de chargement |
| saveOptions | LowCodeSaveOptions | Options de sortie et d'enregistrement |
| provider | AbstractLowCodeProtectionProvider | Implémentation pour fournir les paramètres de protection |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetLockerMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo1
    {
        public static void Run()
        {
           
            // Préparer LowCodeLoadOptions
            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            loadOptions.InputFile = "input.xlsx";

            // Préparer LowCodeSaveOptions
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
            saveOptions.SaveFormat = SaveFormat.Xlsx;
            saveOptions.OutputFile = "output.xlsx";

            // Créer un fournisseur de protection personnalisé
            CustomProtectionProvider provider = new CustomProtectionProvider();

            try
            {
                // Appelez la méthode statique Process avec les paramètres spécifiés
                SpreadsheetLocker.Process(loadOptions, saveOptions, provider);

                Console.WriteLine("Spreadsheet processed and protected successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error processing spreadsheet: {ex.Message}");
            }

        }

        private class CustomProtectionProvider : AbstractLowCodeProtectionProvider
        {
            public override string GetOpenPassword()
            {
                return "open123";
            }

            public override string GetWritePassword()
            {
                return "write123";
            }

            public override string GetWorkbookPassword()
            {
                return "workbook123";
            }

            public override ProtectionType GetWorkbookProtectionType()
            {
                return ProtectionType.All;
            }
        }
    }
}
```

### Voir aussi

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [AbstractLowCodeProtectionProvider](../../abstractlowcodeprotectionprovider/)
* class [SpreadsheetLocker](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


