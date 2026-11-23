---
title: "Worksheet.Unprotect"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Worksheet. Déprotège la feuille de calcul"
type: docs
url: /fr/net/aspose.cells/worksheet/unprotect/
---
## Unprotect() {#unprotect}

Supprime la protection de la feuille de calcul.

```csharp
public void Unprotect()
```

### Remarques

Cette méthode déprotège la feuille de calcul qui est protégée sans mot de passe.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodUnprotectDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Protéger la feuille de calcul avec un mot de passe
            worksheet.Protect(ProtectionType.All, "password123", null);
            Console.WriteLine("Worksheet is protected: " + worksheet.IsProtected);
            
            try
            {
                // Déprotéger la feuille de calcul sans mot de passe (devrait échouer)
                worksheet.Unprotect();
                Console.WriteLine("Worksheet unprotected without password: " + !worksheet.IsProtected);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error when trying to unprotect without password: " + ex.Message);
            }

            try
            {
                // Déprotéger la feuille de calcul avec un mauvais mot de passe (devrait échouer)
                worksheet.Unprotect("wrongpassword");
                Console.WriteLine("Worksheet unprotected with wrong password: " + !worksheet.IsProtected);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error when trying to unprotect with wrong password: " + ex.Message);
            }

            try
            {
                // Déprotéger la feuille de calcul avec le mot de passe correct
                worksheet.Unprotect("password123");
                Console.WriteLine("Worksheet successfully unprotected: " + !worksheet.IsProtected);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error when trying to unprotect: " + ex.Message);
            }
            
            // Enregistrer le résultat
            workbook.Save("WorksheetMethodUnprotectDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Unprotect(string) {#unprotect_1}

Supprime la protection de la feuille de calcul.

```csharp
public void Unprotect(string password)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| mot de passe | String | Mot de passe |

### Remarques

Si la feuille de calcul est protégée sans mot de passe, vous pouvez définir une valeur nulle ou une chaîne vide pour le paramètre mot de passe.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodUnprotectWithStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Protéger la feuille de calcul avec un mot de passe et le type de protection par défaut
            worksheet.Protect(ProtectionType.All, "test", null);
            
            // Déprotéger la feuille de calcul avec le mot de passe
            worksheet.Unprotect("test");
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


