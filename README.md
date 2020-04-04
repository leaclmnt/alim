//Projet alim. Stratégies d'adaptation du repas sans protéines animales ?

//Script

//Session 1 Bloc 1

PennController.ResetPrefix(null);

newTrial(
    defaultText
        .print()
    ,
    newText("Vous allez composer votre premier menu. Pour le plat principal, veuillez choisir un ou plusieurs aliments parmi les suivants :")
    ,
    newButton("Suivant")
        .print()
        .wait()
    ,
)

newTrial(
    newText("Pour l'entr\u00e9e, veuillez choisir une option parmi les quatre propos\u00e9es :")
        .print()
    ,
    newButton("Suivant")
        .print()
        .wait()
)

newTrial(
    newText("Souhaitez-vous un assortiment de fromage ?")
        .print()
    ,
    newButton("Suivant")
        .print()
        .wait()
)

newTrial(
    newText("Vous pouvez maintenant choisir jusqu'à deux desserts parmi les suivants :")
        .print()
    ,
    newButton("Suivant")
        .print()
        .wait()
)

newTrial(
    newText("Vous pouvez choisir une boisson parmi celles propos\u00e9es (vous avez toujours de l'eau plate \u00e0 disposition)")
        .print()
    ,
    newButton("Suivant")
        .print()
        .wait()
)


//Session 1 bloc 2
newTrial(
    newText("Vous allez composer votre second menu. Pour le plat principal, veuillez choisir un ou plusieurs aliments parmi les suivants :")
        .print()
    ,
    newButton("Suivant")
        .print()
        .wait()
    ,
)

newTrial(
    newText("Pour l'entr\u00e9e, veuillez choisir une option parmi les quatre propos\u00e9es :")
        .print()
    ,
    newButton("Suivant")
        .print()
        .wait()
)

newTrial(
    newText("Souhaitez-vous un assortiment de fromage ?")
        .print()
    ,
    newButton("Suivant")
        .print()
        .wait()
)

newTrial(
    defaultText
        .print()
    ,
    newText("Vous pouvez maintenant choisir jusqu'à deux desserts parmi les suivants :")
    ,
    newButton("Suivant")
        .print()
        .wait()
)

newTrial(
    newText("Vous pouvez choisir une boisson parmi celles propos\u00e9es (vous avez toujours de l'eau plate \u00e0 disposition)")
        .print()
    ,
    newButton("Suivant")
        .print()
        .wait()
)




//Message d'encouragement
newTrial(
    newText("Courage, vous \u00eates presque à la fin du questionnaire !")
        .print()
    ,
    newButton("Poursuivre")
        .print()
        .wait()
)

