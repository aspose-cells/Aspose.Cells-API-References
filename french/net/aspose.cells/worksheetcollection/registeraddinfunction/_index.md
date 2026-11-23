---
title: "WorksheetCollection.RegisterAddInFunction"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode WorksheetCollection. Ajoute une fonction addin au classeur"
type: docs
url: /fr/net/aspose.cells/worksheetcollection/registeraddinfunction/
---
## RegisterAddInFunction(string, string, bool) {#registeraddinfunction}

Ajoute la fonction d'add‑in dans le classeur

```csharp
public int RegisterAddInFunction(string addInFile, string functionName, bool lib)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| addInFile | String | le fichier contient les fonctions addin |
| functionName | String | le nom de la fonction addin |
| lib | Boolean | indique si le fichier addin fourni se trouve dans le répertoire ou sous‑répertoire de Workbook Add‑In library. Ce drapeau prend effet et fait une différence lorsque le addInFile fourni est un chemin relatif : true indique que le chemin est relatif à Add‑In library et false indique que le chemin est relatif à ce Workbook. |

### Valeur de retour

ID des données contenant la fonction addin donnée

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodRegisterAddInFunctionWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook wb = new Workbook();
            
            // Obtenir la première feuille de calcul
            Worksheet sheet = wb.Worksheets[0];
            
            // Définir les chemins de fichiers d'exemple (ils doivent exister dans votre environnement)
            string addInFile1 = Path.Combine("AddIns", "MyAddIn1.xlam");
            string addInFile2 = Path.Combine("AddIns", "MyAddIn2.xlam");
            
            // Enregistrer les fonctions add‑in avec différents paramètres
            int id1 = wb.Worksheets.RegisterAddInFunction(addInFile1, "MY_UDF1", false);
            int id2 = wb.Worksheets.RegisterAddInFunction(addInFile2, "MY_UDF2", true);
            
            // Utiliser les fonctions enregistrées dans les cellules
            sheet.Cells["A1"].Formula = "=MY_UDF1()";
            sheet.Cells["A2"].Formula = "=MY_UDF2()";
            
            // Enregistrez le classeur
            wb.Save("RegisterAddInFunctionDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RegisterAddInFunction(int, string) {#registeraddinfunction_1}

Ajoute la fonction d'add‑in dans le classeur

```csharp
public string RegisterAddInFunction(int id, string functionName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| id | Int32 | ID des données qui contiennent les fonctions d'add‑in, peut être obtenu lors du premier appel de `RegisterAddInFunction` pour le même fichier d'add‑in. |
| functionName | String | le nom de la fonction addin |

### Valeur de retour

URL du fichier d'add‑in qui contient les fonctions d'add‑in

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodRegisterAddInFunctionWithInt32StringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Enregistrer la première fonction d'add‑in et obtenir son ID
            int functionId = workbook.Worksheets.RegisterAddInFunction("externallink1.xlam", "customfunc1", false);
            
            // Enregistrer la deuxième fonction d'add‑in en utilisant le même ID
            workbook.Worksheets.RegisterAddInFunction(functionId, "customfunc2");
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Utiliser les fonctions enregistrées dans les formules
            cells["A1"].Formula = "=customfunc1()";
            cells["A2"].Formula = "=customfunc2()";
            
            // Enregistrez le classeur
            workbook.Save("RegisterAddInFunctionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


