---
title: "Validation.AddArea"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Validation. Applica la convalida all'area"
type: docs
url: /it/net/aspose.cells/validation/addarea/
---
## AddArea(CellArea) {#addarea}

Applica la convalida all'area.

```csharp
public void AddArea(CellArea cellArea)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellArea | CellArea | L'area. |

### Osservazioni

È equivalente usare `AddArea` con il controllo dell'intersezione e del bordo.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodAddAreaWithCellAreaDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Crea una convalida
            ValidationCollection vc = sheet.Validations;
            Validation validation = vc[vc.Add(CellArea.CreateCellArea(0, 0, 0, 0))];
            validation.Type = ValidationType.List;
            validation.Formula1 = "=A1:A10";

            // Aggiungi più aree alla convalida
            for (int i = 1; i < 5; i++)
            {
                validation.AddArea(CellArea.CreateCellArea(i, 0, i, 0));
            }

            // Salva la cartella di lavoro
            wb.Save("ValidationMethodAddAreaWithCellAreaDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("Validation with multiple areas created successfully.");
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddArea(CellArea, bool, bool) {#addarea_1}

Applica la convalida all'area.

```csharp
public void AddArea(CellArea cellArea, bool checkIntersection, bool checkEdge)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellArea | CellArea | L'area. |
| checkIntersection | Booleano | Indica se verificare l'intersezione dell'area fornita con le aree delle convalide esistenti. Se una convalida è stata applicata nell'area fornita (o in una sua parte), allora la convalida esistente dovrebbe essere rimossa prima dall'area fornita. Altrimenti potrebbe verificarsi corruzione per le Validations generate. Se l'utente è sicuro che l'area aggiunta non si intersechi con alcuna area esistente, questo parametro può essere impostato su false per considerazioni di prestazioni. |
| checkEdge | Booleano | Indica se verificare il bordo delle aree a cui è applicata questa convalida. Le impostazioni interne della Validation dipendono dall'area in alto a sinistra delle sue intervalli applicati, quindi se l'area fornita diventerà la nuova area in alto a sinistra degli intervalli applicati, le impostazioni interne devono essere modificate e ricostruite, altrimenti potrebbero verificarsi risultati inattesi. Se l'utente è sicuro che l'area aggiunta non sia quella in alto a sinistra, questo parametro può essere impostato su false per considerazioni di prestazioni. |

### Osservazioni

In questo metodo, rimuoveremo tutte le vecchie convalide nell'area fornita. Per l'area in alto a sinistra degli intervalli applicati di Validation, prima il suo StartRow è il più piccolo, poi il suo StartColumn è il più piccolo tra le aree che hanno lo stesso StartRow minimo.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodAddAreaWithCellAreaBooleanBooleanDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una convalida in un'area specifica
            Validation validation = worksheet.Validations[worksheet.Validations.Add(CellArea.CreateCellArea(5, 3, 6, 3))];
            validation.Operator = OperatorType.GreaterThan;
            validation.Formula1 = "F3";

            // Dimostra AddArea con CellArea e due parametri booleani
            validation.AddArea(CellArea.CreateCellArea(3, 3, 3, 4), false, true);
            Console.WriteLine("Area count after AddArea: " + validation.Areas.Length);
            Console.WriteLine("Formula1 after AddArea: " + validation.Formula1);

            // Rimuovi l'area aggiunta
            validation.RemoveArea(CellArea.CreateCellArea(3, 3, 3, 4));
            Console.WriteLine("Area count after RemoveArea: " + validation.Areas.Length);

            // Aggiungi più aree con un'operazione di massa
            CellArea[] areas = new CellArea[10];
            for (int i = 0; i < areas.Length; i++)
            {
                areas[i] = CellArea.CreateCellArea(6 + i, 3, 6 + i, 4);
            }
            validation.AddAreas(areas, true, true);
            Console.WriteLine("Area count after bulk AddAreas: " + validation.Areas.Length);

            // Salva la cartella di lavoro
            workbook.Save("ValidationMethodAddAreaDemo.xlsx");
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


