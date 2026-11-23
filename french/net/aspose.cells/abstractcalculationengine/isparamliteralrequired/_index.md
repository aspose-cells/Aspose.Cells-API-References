---
title: "AbstractCalculationEngine.IsParamLiteralRequired"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété AbstractCalculationEngine. Indique si ce moteur a besoin du texte littéral du paramètre lors d'un calcul. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells/abstractcalculationengine/isparamliteralrequired/
---
## AbstractCalculationEngine.IsParamLiteralRequired property

Indique si ce moteur a besoin du texte littéral du paramètre lors d'un calcul. La valeur par défaut est false.

```csharp
public virtual bool IsParamLiteralRequired { get; }
```

### Remarques

Si ce moteur de calcul personnalisé a besoin du texte littéral du paramètre, davantage de piles seront nécessaires pour mettre en cache le texte littéral des paramètres et la méthode Calculate() pourra être appelée de manière récursive pour calculer la valeur du paramètre. En général, le texte littéral n'est pas nécessaire pour le calcul des formules et cette propriété doit rester à false pour la plupart des implémentations afin d'obtenir de meilleures performances.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractCalculationEnginePropertyIsParamLiteralRequiredDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une instance de moteur de calcul personnalisé
            MyCustomEngine engine = new MyCustomEngine();

            // Lire la valeur actuelle de la propriété
            Console.WriteLine("Current IsParamLiteralRequired value: " + engine.IsParamLiteralRequired);

            // Créer une formule de test avec un paramètre littéral de chaîne
            worksheet.Cells["A1"].Formula = "=MYFUNC(\"123\")";

            // Calculer le classeur avec des options de calcul personnalisées
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = engine;
            workbook.CalculateFormula(options);

            // Afficher le résultat du calcul basé sur la valeur de la propriété
            Console.WriteLine("Formula result: " + worksheet.Cells["A1"].StringValue);

            workbook.Save("IsParamLiteralRequiredDemo.xlsx");
        }
    }

    public class MyCustomEngine : AbstractCalculationEngine
    {
        public override bool IsParamLiteralRequired => true;

        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName.Equals("MYFUNC", StringComparison.OrdinalIgnoreCase))
            {
                if (data.ParamCount > 0)
                {                    
                    object paramValue = data.GetParamValue(0);
                    string result = (paramValue is string) ? "Literal received" : "Value received";
                    data.CalculatedValue = result;
                }
            }
        }
    }
}
```

### Voir aussi

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


