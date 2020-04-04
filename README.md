//Projet alim. Stratégies d'adaptation du repas sans protéines animales ?

//Script

//Intro
PennController.ResetPrefix(null) // Shorten command names (keep this line here)

PennController(
    newText("Bonjour,")
        .print()
    ,
    newText("Dans le cadre d’un projet de recherche à AgroParisTech, nous souhaiterions que vous répondiez à un questionnaire, qui vous prendra environ 10 minutes. ")
        .print()
    ,
    newText("Cela nous aidera beaucoup pour nos recherches. Le questionnaire est anonyme, et les données collectées sont stockées dans une base de données sécurisées.")
        .print()
    ,
    newText("Pour toute question ou commentaire, vous pouvez nous contacter à l’adresse suivante : ??.")
        .print()
    ,
    newButton("Suivant")
        .print()
        .wait()
)


PennController(
    newText("Vous allez composer différents menus, à chaque fois pour un repas à domicile.")
        .print()
    ,
    newText("Pour chaque catégorie (plat principal, entrée, fromage, dessert, boisson), vous allez pouvoir choisir un ou plusieurs aliments.")
        .print()
    ,
    newText("Dans tous les cas, il y a à disposition de l’eau plate, du pain, des condiments, des épices.")
        .print()
    ,
    newButton("Suivant")
        .print()
        .wait()
)

//Session 1 Bloc 1
PennController.ResetPrefix(null);

newTrial(
    defaultText
        .print()
    ,
    newText("Vous allez composer votre premier menu. Pour le plat principal, veuillez choisir un ou plusieurs aliments parmi les suivants :")
    ,
    newButton("Passer à l'entr\u00e9e")
        .print()
        .wait()
    ,
)

newTrial(
    newText("Pour l'entr\u00e9e, veuillez choisir une option parmi les quatre propos\u00e9es :")
        .print()
    ,
    newButton("Passer au fromage")
        .print()
        .wait()
)

newTrial(
    newText("Souhaitez-vous un assortiment de fromage ?")
        .print()
    ,
    newButton("Passer au dessert")
        .print()
        .wait()
)

newTrial(
    newText("Vous pouvez maintenant choisir jusqu'\u00e0 deux desserts parmi les suivants :")
        .print()
    ,
    newButton("Passer à la boisson")
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
    newButton("Passer à l'entr\u00e9e")
        .print()
        .wait()
    ,
)

newTrial(
    newText("Pour l'entr\u00e9e, veuillez choisir une option parmi les quatre propos\u00e9es :")
        .print()
    ,
    newButton("Passer au fromage")
        .print()
        .wait()
)

newTrial(
    newText("Souhaitez-vous un assortiment de fromage ?")
        .print()
    ,
    newButton("Passer au dessert")
        .print()
        .wait()
)

newTrial(
    defaultText
        .print()
    ,
    newText("Vous pouvez maintenant choisir jusqu'\u00e0 deux desserts parmi les suivants :")
    ,
    newButton("Passer à la boisson")
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


//Session 2


//Message d'encouragement
newTrial(
    newText("Courage, vous \u00eates presque \u00e0 la fin du questionnaire !")
        .print()
    ,
    newButton("Poursuivre")
        .print()
        .wait()
)



//Session 3
