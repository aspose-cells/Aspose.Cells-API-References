---
title: "VbaModuleCollection.AddUserForm"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "VbaModuleCollection-Methode. Benutzerformular in das VBA-Projekt einfügen"
type: docs
url: /de/net/aspose.cells.vba/vbamodulecollection/adduserform/
---
## VbaModuleCollection.AddUserForm method

Benutzerformular in das VBA-Projekt einfügen.

```csharp
public int AddUserForm(string name, string codes, byte[] designerStorage)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | String | Der Name des Benutzerformulars |
| Codes | String | Die Codes für das Benutzerformular |
| designerStorage | Byte[] | die Designer-Einstellung für das Benutzerformular |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das VBA-Projekt
            VbaProject vbaProject = workbook.VbaProject;
            VbaModuleCollection vbaModules = vbaProject.Modules;

            // Parameter für AddUserForm vorbereiten
            string formName = "UserForm1";
            string formCode = 
                "Private Sub CommandButton1_Click()\n" +
                "    MsgBox \"Hello from UserForm!\"\n" +
                "End Sub";
            
            // Einfachen Designer-Speicher erstellen (dies wäre normalerweise die .frx-Binärdaten)
            byte[] designerStorage = new byte[] { 0x00, 0x01, 0x02, 0x03 };

            try
            {
                // AddUserForm mit (String, String, Byte[])-Parametern aufrufen
                int moduleIndex = vbaModules.AddUserForm(formName, formCode, designerStorage);
                
                Console.WriteLine($"UserForm added successfully at index: {moduleIndex}");
                Console.WriteLine($"Total VBA modules: {vbaModules.Count}");

                // Speichern Sie das Arbeitsbuch, um die Änderungen am VBA-Projekt zu sehen
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

### Siehe auch

* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


