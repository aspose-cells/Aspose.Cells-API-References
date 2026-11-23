---
title: "VbaModuleCollection.AddUserForm"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode VbaModuleCollection. Insérer un formulaire utilisateur dans le projet VBA"
type: docs
url: /fr/net/aspose.cells.vba/vbamodulecollection/adduserform/
---
## VbaModuleCollection.AddUserForm method

Insérer le formulaire utilisateur dans le projet VBA.

```csharp
public int AddUserForm(string name, string codes, byte[] designerStorage)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Le nom du formulaire utilisateur |
| codes | String | Les codes du formulaire utilisateur |
| designerStorage | Byte[] | les paramètres du concepteur du formulaire utilisateur |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;
    using System.IO;

    public class VbaModuleCollectionMethodAddUserFormWithStringStringByteDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder au projet VBA
            VbaProject vbaProject = workbook.VbaProject;
            VbaModuleCollection vbaModules = vbaProject.Modules;

            // Préparer les paramètres pour AddUserForm
            string formName = "UserForm1";
            string formCode = 
                "Private Sub CommandButton1_Click()\n" +
                "    MsgBox \"Hello from UserForm!\"\n" +
                "End Sub";
            
            // Créer un stockage de concepteur simple (cela serait normalement les données binaires .frx)
            byte[] designerStorage = new byte[] { 0x00, 0x01, 0x02, 0x03 };

            try
            {
                // Appeler AddUserForm avec les paramètres (String, String, Byte[])
                int moduleIndex = vbaModules.AddUserForm(formName, formCode, designerStorage);
                
                Console.WriteLine($"UserForm added successfully at index: {moduleIndex}");
                Console.WriteLine($"Total VBA modules: {vbaModules.Count}");

                // Enregistrez le classeur pour voir les modifications du projet VBA
                workbook.Save("AddUserFormDemo.xlsm", SaveFormat.Xlsm);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding UserForm: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


