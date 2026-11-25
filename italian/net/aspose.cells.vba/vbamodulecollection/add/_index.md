---
title: "VbaModuleCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo VbaModuleCollection. Aggiunge un modulo per un foglio di lavoro"
type: docs
url: /it/net/aspose.cells.vba/vbamodulecollection/add/
---
## Add(Worksheet) {#add_1}

Aggiunge un modulo per un foglio di lavoro.

```csharp
public int Add(Worksheet sheet)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| foglio | Worksheet | Il foglio di lavoro |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaModuleCollectionMethodAddWithWorksheetDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi un modulo VBA associato al foglio di lavoro
            int moduleIndex = workbook.VbaProject.Modules.Add(worksheet);
            
            // Aggiungi del codice VBA al modulo
            string vbaCode = "Sub Test()\n    MsgBox \"Hello from VBA!\"\nEnd Sub";
            workbook.VbaProject.Modules[moduleIndex].Codes = vbaCode;
            
            // Salva la cartella di lavoro con il progetto VBA
            workbook.Save("output.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### Vedi anche

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)

---

## Add(VbaModuleType, string) {#add}

Aggiunge un modulo.

```csharp
public int Add(VbaModuleType type, string name)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | VbaModuleType | Il tipo di modulo. |
| name | String | Il nome del modulo. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModuleCollectionMethodAddWithVbaModuleTypeStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            VbaProject vbaProject = workbook.VbaProject;

            int index = vbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
            VbaModule module = vbaProject.Modules[index];
            module.Codes = "Sub Test()\r\nMsgBox \"Hello World\"\r\nEnd Sub";

            workbook.Save("VbaModuleAddExample.xlsm");
        }
    }
}
```

### Vedi anche

* enum [VbaModuleType](../../vbamoduletype/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


