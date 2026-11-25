---
title: "MsoFillFormatHelper.SetOneColorGradient"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo MsoFillFormatHelper. Imposta il riempimento specificato a un gradiente a un colore"
type: docs
url: /it/net/aspose.cells.drawing/msofillformathelper/setonecolorgradient/
---
## MsoFillFormatHelper.SetOneColorGradient method

Imposta il riempimento specificato a un gradiente a un colore.

```csharp
public void SetOneColorGradient(Color color, double degree, GradientStyleType style, int variant)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colore | Color | Un colore di gradiente. |
| grado | Double | Il grado del gradiente. Può essere un valore da 0.0 (scuro) a 1.0 (chiaro). |
| stile | GradientStyleType | Stile di sfumatura del gradiente. |
| variant | Int32 | La variante del gradiente. Può essere un valore da 1 a 4, corrispondente a una delle quattro varianti nella scheda Gradient del dialogo Effetti di riempimento. Se lo stile è GradientStyle.FromCenter, l'argomento Variant può essere solo 1 o 2. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatHelperMethodSetOneColorGradientWithColorDoubleGradientStyleTyInt32Demo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Inserisci un'etichetta semplice nel foglio per contesto
            worksheet.Cells["A1"].Value = "Gradient Fill Demo";

            try
            {
                // Crea un'istanza di MsoFillFormatHelper usando la riflessione (senza costruttore pubblico)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Parametri per il gradiente
                Color gradientColor = Color.FromArgb(255, 0, 120, 215); // a shade of blue
                double degree = 45.0;                                 // gradient angle in degrees
                GradientStyleType style = GradientStyleType.Horizontal; // horizontal gradient
                int variant = 0;                                      // variant (0 = default)

                // Applica il gradiente a un colore
                fillHelper.SetOneColorGradient(gradientColor, degree, style, variant);

                // Opzionale: mostra che le proprietà possono essere lette dopo la chiamata
                Console.WriteLine($"ForeColor after gradient: {fillHelper.ForeColor}");
                Console.WriteLine($"ForeColorTransparency after gradient: {fillHelper.ForeColorTransparency}");

                // Salva la cartella di lavoro (non verrà visualizzato alcun cambiamento perché l'helper non è collegato a una forma)
                workbook.Save("SetOneColorGradientDemo.xlsx");

                Console.WriteLine("SetOneColorGradient method called successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetOneColorGradient: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [GradientStyleType](../../gradientstyletype/)
* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


