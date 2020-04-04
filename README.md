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

//Questions complémentaires
<table>
<tr>
<td colspan="2" style="padding-bottom: 1em;"><input type="checkbox" class="obligatory" name="consent" id="consentcx" /><label for="consentcx"> Je consens à remplir ce questionnaire </label></td>
</tr>
<tr>
<td colspan="2">
<label class="error" for="consent"></label>
</td>
</tr>
<tr>
  <td>Nom:</td><td><input name="name" type="text" size="30" class="obligatory" /></td>
</tr>
<tr>
<td colspan="2"><label class="error" for="name"></label></td>
</tr>
<tr>
  <td>Âge:</td><td><input name="age" type="text" size="30" class="obligatory" /></td>
</tr>
<tr>
<td colspan="2"><label class="error" for="age"></label></td>
</tr>
<tr>
  <td>Sexe:</td><td><input name="sex" type="radio" value="male" class="obligatory" id="csexmale" /><label for="csexmale">Homme </label>
                   <input name="sex" type="radio" value="female" id="csexfemale"/><label for="csexfemale"> Femme</label>
                   <input name="sex" type="radio" value="autre" id="csexautre"/><label for="csexautre"> Autre</label>
</tr>
<tr>
<td colspan="2"><label class="error" for="sex"></label></td>
</tr>
<tr>
<tr>
<td colspan="2"><label class="error" for="religion"></label></td>
</tr>
<tr>
<tr>
<td>Régime:</td><td><input name="regime" type="radio" value="Omnivore" class="obligatory" id="cregimeomnivore" /><label for="cregimeomnivore">Omnivore </label>
                   <input name="regime" type="radio" value="Vegetarien" id="cregimevegetarien"/><label for="cregimevegetarien"> Végétarien</label>
                   <input name="regime" type="radio" value="Vegetalien" id="cregimevegetalien"/><label for="cregimevegetalien"> Végétalien</label>
</tr>
<tr>
<td colspan="2"><label class="error" for="regime"></label></td>
</tr>
<tr>
  <td colspan="2">Quelle est votre catégorie socio-professionnelle ? </td>
</tr>
<tr>
  <td colspan="2">
    <textarea name="Categoriesocio-pro" rows="1" cols="30"></textarea>
  </td>
</tr>
<tr>
  <td colspan="2"> Pratiquez-vous une activité sportive régulière ? (si oui, à quelle fréquence) </td>
</tr>
<tr>
  <td colspan="2">
    <textarea name="sport" rows="1" cols="30"></textarea>
  </td>
</tr>
<tr>
  <td colspan="2"> Êtes-vous satisfait de votre poids ? (répondez par oui ou par non)</td>
</tr>
<tr>
  <td colspan="2">
    <textarea name="satisfait" rows="1" cols="30"></textarea>
  </td>
</tr>
<tr>
<td colspan="2"> Êtes-vous issu d’un milieu rural ou urbain ? (répondez par oui ou par non)</td>
</tr>
<tr>
  <td colspan="2">
    <textarea name="satisfait" rows="1" cols="30"></textarea>
  </td>
</tr>
