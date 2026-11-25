---
title: "VbaModuleCollection.AddUserForm"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo VbaModuleCollection. Inserisci form utente nel progetto VBA"
type: docs
url: /it/net/aspose.cells.vba/vbamodulecollection/adduserform/
---
## VbaModuleCollection.AddUserForm method

Inserisci il modulo utente nel progetto VBA.

```csharp
public int AddUserForm(string name, string codes, byte[] designerStorage)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome del form utente |
| codici | String | I codici per il form utente |
| designerStorage | Byte[] | l'impostazione del designer per il form utente |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al progetto VBA
            VbaProject vbaProject = workbook.VbaProject;
            VbaModuleCollection vbaModules = vbaProject.Modules;

            // Prepara i parametri per AddUserForm
            string formName = "UserForm1";
            string formCode = 
                "Private Sub CommandButton1_Click()\n" +
                "    MsgBox \"Hello from UserForm!\"\n" +
                "End Sub";
            
            // Crea un semplice archivio del designer (questo sarebbe normalmente il dato binario .frx)
            byte[] designerStorage = new byte[] { 0x00, 0x01, 0x02, 0x03 };

            try
            {
                // Chiama AddUserForm con i parametri (String, String, Byte[])
                int moduleIndex = vbaModules.AddUserForm(formName, formCode, designerStorage);
                
                Console.WriteLine($"UserForm added successfully at index: {moduleIndex}");
                Console.WriteLine($"Total VBA modules: {vbaModules.Count}");

                // Salva la cartella di lavoro per vedere le modifiche al progetto VBA
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

### Vedi anche

* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


