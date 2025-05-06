---
title: AutoFitterOptions.MaxRowHeight
second_title: Aspose.Cells for .NET API Reference
description: AutoFitterOptions property. Gets and sets the max row heightin unit of Point when autofitting rows
type: docs
url: /net/aspose.cells/autofitteroptions/maxrowheight/
---
## AutoFitterOptions.MaxRowHeight property

Gets and sets the max row height(in unit of Point) when autofitting rows.

```csharp
public double MaxRowHeight { get; set; }
```

### Examples

```csharp
// Called: options.MaxRowHeight = 255;
[Test]
        public void Property_MaxRowHeight()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet42275.XLS&quot;);


            string f1 = &quot;Data1&quot;;

            string f2 = &quot;Data2&quot;;

            string f3 = &quot;Data3&quot;;

            string f4 = &quot;Data4&quot;;

            string f5 = &quot;C&apos;est trop long......je n&apos;ai a ce jour  rien reçu pour ma maison....puisque nous sommes plusieurs habitations  affectées par la grêle, je suis la seule a n&apos;avoir rien reçu encore.....ma soeur cela fait 2 semaines qu&apos;elle a sont chèque malgré que c&apos;était un gros montant 18,000.00 ça été vite elle a commencer c&apos;est travaux, car l&apos;hiver  arrive moi je vais être obligé d&apos;attendre l&apos;année prochaine..... J&apos;ai tenté d&apos;aider le règlement en demandant des soumissions pour les gouttières et le solin, portes-patios, ils ont tout entre les mains et rien encore, nous sommes le 23 octobres.  J&apos;ai commandé les portes-patios le 3 octobre, car ils faux que je les change avant l&apos;hiver et ici cela prend 3 semaines pour les commander je devrais les avoir aujourd&apos;hui.....aussitôt qu&apos;il fait plus chaud je vais les changer.....  Même s&apos; il y avait beaucoup de réclamation après 1 mois   devrait être réglé, ils sont entre les mains tout ce qu&apos;il faut.    Pour la voiture cela a été vite, le degrailleur était sur place, par téléphone ont ma donné un rendez-vous.... par contre ma voiture est neuve....acheté le 11 janvier 2013... si vous regardé dans mon dossier vous serez capable de voir que c&apos;est ma première voiture neuve et que les autres voitures étaient usagées ( j&apos;ai toujours été assuré chez vous depuis début année 1980.  De plus je garde mes voitures toujours plus de 10 ans.   Puisqu&apos;ils ont dû repeindre certaine partit de ma voiture, je me suis posé la question la garantie de ma peinture d&apos;origine ne sera plus valide...j&apos;ai téléphone a la compagnie assurance pour avoir les renseignements qu&apos;elle partit au juste avait été repeinturé, la semaine passé ( laisser message sur le répondeur de Messieur Dubé) rien reçu à date. C&apos;est pour savoir si commence a rouiller pour les garanties..... si de la rouilles commence a sortir, est ce la peinture d&apos;origine qui est pas bonne ou c&apos;elle qui a été peinturée.. c&apos;est important pour moi.... j&apos;avais même indiqué de laisser le message sur mon répondeur si je n&apos;étais pas la.   Ma voiture Trax Manuel ( $ 19,948.00 )  il y a eue pour près de 11,000.00.    Je viens d&apos;aller à la poste  et pas reçu de renseignements, ma soeur pour le camion sa compagnie lui a remis sur papier toutes les réparations qui ont été effectuées ( il en avait pour 9000.00).    Je vais peut-être recevoir tout ça par la poste bientôt le chèque et documents.....           Je n&apos;avais jamais fait de réclamation, je pensais qu&apos;après 2 ou 3 semaines au maximum tout serait réglé....et bien non pour moi  et d&apos;autre qui sont assuré chez vous, j&apos;ai un oncle que c&apos;est les bardeaux (toit) de sa maison qui sont a changé et  la semaine passée n&apos;avait rien reçu encore.....  Pour moi, je peux dire que j&apos;avais changé mes bardeaux l&apos;année passée par chance...tout semble correct....par chance aussi que ma maison est en brique si nom comme mes voisins tout leur revêtement de maison est a changé....je n&apos;ai pas eu de fenêtre de cassée par chance, certains de mes voisins oui....Ce qui est arrivé avec de la grêle comme des oranges et pamplemousse est très rare et beaucoup de monde ont été affecté, mais pour les autres compagnies tout est terminé...réglé et la votre non, pour vous aidez j&apos;ai même envoyé des soumissions, etc.. que puisje faire de plus.. attendre.... je vais allé au bureau de poste demain......nous sommes le 23 octobre 2013 1h30 pm.&quot;;

            StringBuilder sb = new StringBuilder();


            int maxLineToAdd = 45;

            for (int i = 0; i &lt; maxLineToAdd; i++)
            {

                sb.AppendFormat(&quot;Line {0:000} text without any line break. text without any line break. text&quot;, i);

            }


            Worksheet worksheet = workbook.Worksheets[&quot;Presentation&quot;];


            worksheet.Cells[4, 0].PutValue(f1);

            worksheet.Cells[4, 1].PutValue(f2);

            worksheet.Cells[4, 2].PutValue(f3);

            worksheet.Cells[4, 3].PutValue(f4);

            worksheet.Cells[4, 4].PutValue(sb.ToString());

            AutoFitterOptions options = new AutoFitterOptions();
            options.MaxRowHeight = 255;
            worksheet.AutoFitRows(options);
            Assert.AreEqual(worksheet.Cells.GetRowHeight(4), 255);
        }
```

### See Also

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


