---
title: "WorkbookSettings.IsProtected"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Restituisce un valore che indica se la struttura o la finestra della cartella di lavoro è protetta"
type: docs
url: /it/net/aspose.cells/workbooksettings/isprotected/
---
## WorkbookSettings.IsProtected property

Ottiene un valore che indica se la struttura o la finestra del Workbook è protetta.

```csharp
public bool IsProtected { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsProtectedDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi alle impostazioni della cartella di lavoro
            WorkbookSettings settings = workbook.Settings;
            
            // Verifica se la cartella di lavoro è protetta
            Console.WriteLine("Workbook is protected: " + settings.IsProtected);
            
            // Proteggi la cartella di lavoro con una password
            settings.Password = "password123";
            
            // Verifica lo stato della protezione
            Console.WriteLine("Workbook is protected: " + settings.IsProtected);
            
            // Salva la cartella di lavoro protetta
            workbook.Save("ProtectedWorkbook.xlsx", SaveFormat.Xlsx);
            
            // Apri la cartella di lavoro protetta
            Workbook protectedWorkbook = new Workbook("ProtectedWorkbook.xlsx");
            
            // Verifica lo stato di protezione della cartella di lavoro caricata
            Console.WriteLine("Loaded workbook is protected: " + protectedWorkbook.Settings.IsProtected);
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


