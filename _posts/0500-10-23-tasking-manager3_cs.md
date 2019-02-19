---
layout: doc
title: Tasking Manager 3
permalink: /cs/coordination/tasking-manager3/
lang: cs
category: coordination
---

# Tasking Manager 3

> Tento návod může být stažen jako [tasking-manager3_en.odt](/files/tasking-manager3_en.odt) nebo [tasking-manager3_en.pdf](/files/tasking-manager3_en.pdf)  

**Tento návod popisuje aktuální verzi Tasking Manageru. Pokud uživatelské rozhraní, které používáte, vypadá jinak než zde popsané, měli byste si prohlédnout [příručku pro předchozí verzi](/cs/coordination/tasking-manager)**

Sekce Index
-------------
- [Rychlý návod](/cs/coordination/tasking-manager3/#quick-start-guide)  
- [Proces mapování](/cs/coordination/tasking-manager3/#mapping-process)  
    - [Přihlašování](/cs/coordination/tasking-manager3/#tasking-manager-login)  
    - [Možnosti - nastavení jazyka a uživatelský profil](/cs/coordination/tasking-manager3/#options-amp-links)  
    - [Vyhledání projektu založeného na seznamu a používání zobrazení mapy, vyhledávání a filtrování](/cs/coordination/tasking-manager3/#finding-a-project---tasking-manager-contribute-screen)  
    - [Mapování úlohy - vyberte, pracujte a odemkněte úkol](/cs/coordination/tasking-manager3/#mapping-via-the-tasking-manager) 
- [Získání nápovědy - naživo a kontaktování správce projektu](/cs/coordination/tasking-manager3/#getting-help)  
- [Tipy a triky](/cs/coordination/tasking-manager3/#editing-hints-and-tips)
- [Validace](/cs/coordination/tasking-manager3/#validation)

[HOT OSM Tasking Manager](http://tasks.hotosm.org) je nástroj, který koordinuje mnoho lidí mapujících určitou geografickou oblast v OpenStreetMapě.

OpenStreetMap je svobodná, bezplatná mapa světa založená na spolupráci. Každý, kdo může přispívat na OpenStreetMap, mapuje libovolnou část světa, která ho zajímá. Tasking Manager je jen způsob, jak koordinovat velké skupiny lidí, kteří přispívají k OpenStreetMap, ale většinu příspěvků k OpenStreetMap dělají lidé, kteří nepoužívají Tasking Manager.

Tasking Manager je zcela samostatný nástroj oddělený od hlavního projektu OpenStreetMap. Když přispíváte k OpenStreetMap pomocí Tasking Manageru, ve skutečnosti používáte několik softwarových nástrojů:

* OpenStreetMap - databáze geografických informací
* Tasking Manager - pomáhá koordinovat velké množství lidí, kteří upravují data OpenStreetMap ve stejné oblasti
* OpenStreetMap Editor - softwarový program, který dokáže číst a zapisovat data do databáze OpenStreetMap

![TM overview][]

Úkolem Tasking Manageru je představit určitou geografickou oblast rozdělenou do malých, rychle mapovatelných oblastí nazvaných "Úkoly" a poskytnout způsob, jak "zabrat" nebo "uzamknout" jednu z těchto malých oblastí, zatímco mapujete tuto oblast pomocí jednoho standardních editorů OpenStreetMap. Tím, že "zaberete" nebo "uzamknete" jednu z těchto malých oblastí, pomůžete zajistit, že nikdo jiný nebude mapovat v téže oblasti, zatímco mapujete. To pomáhá zabránit "dvojitému mapování" nebo jiným chybám, když dva lidé pracují na stejné oblasti v OpenStreetMap.

Po dokončení mapování této malé oblasti zaznamenáváte do Tasking Manageru, že jste dokončili mapování této malé oblasti a doufejme, že si vyberete další "úlohu" na mapování.


## Rychlý návod

1. Vytvořte účet a přihlaste se na http://openstreetmap.org/  
  ![TM Quick Start 1][]
2. Navštivte [http://tasks.hotosm.org/](http://tasks.hotosm.org/) a přihlaste se přes pravý horní roh  
  ![TM Quick Start 2][]
3. Klikněte na "Zapojit se" a najděte mapovací projekt, na který budete pracovat  
  ![TM Quick Start 3][]
4. Přečtěte si pokyny k projektu  
  ![TM Quick Start 4][]
5. Klikněte na kartu "Mapa"  
  ![TM Quick Start 5][]
6. Najděte úkol "Ready", který chcete pracovat, klikněte na něj a vyberte "Start Mapping"  
  ![TM Quick Start 6][]
7. Budete přepojeni na editor OpenStreetMap a můžete mapovat všechny úkoly požadované v instrukcích.  
  ![TM Quick Start 7][]
8. Po dokončení mapování přepněte zpět do Správce úloh a klepnutím na tlačítko "Označit jako úplně zmapováno", pokud jste plně zmapovali úkol nebo "Zastavit mapování", pokud potřebujete z nějakého důvodu zastavit mapování.  
  ![TM Quick Start 8][]


## Proces mapování 

1. Vzdálený mapař vytvoří účet v aplikaci OpenStreetMap a přihlásí se do Tasking Manageru.
1. Mapař najde projekt, na kterém pracuje, obvykle založený na prioritě a úrovni dovedností nastavené správcem projektu v Tasking Manageru. 
2. Vzdálený mapař vybere čtverec úlohy, dokončí mapování a označí úlohu za dokončenou.
3. Druhý vzdálený mapař zkontroluje, zda je úkol dokončen na uspokojivou úroveň a označuje úkol jako "ověřený"
4. Vývoj mapování lze sledovat z tabulky "statistiky" projektu a může být snížena jeho naléhavost nebo být archivován podle požadavků administrátora.

### Přihlášení do Tasking Manageru

Tasking Manager je samostatný nástroj, který koordinuje mapování v OpenStreetMap. Používá však přihlašovací systém OpenStreetMap. To znamená, že k použití Tasking Manageru nemusíte vytvářet samostatný uživatelský účet, musíte však vytvořit účet v OpenStreetMap a přihlásit se do OpenStreetMap před tím, než můžete použít Tasking Manager pro mapování.

Když poprvé navštívíte Tasking Manager, zobrazí se v pravém horním rohu obrazovky tlačítko "Login".

![TM login 1][]

Kliknutím na toto tlačítko se dostanete na webovou stránku OpenStreetMap. Zde budete muset přihlásit a povolit správci Tasking Manager přístup k vašim preferencím OpenStreetMap. Pokud ještě nemáte, vytvořte si účet na webové stránce OpenStreetMap.

![TM login 2][]

![TM login 3][]

Jakmile jste přihlášeni do OpenStreetMap, vrátíte se do Tasking Manageru, kliknutím na Zapojit se, se dostanete k seznamu projektů, do kterých můžete přispět.

### Možnosti a odkazy

Tasking Manager se zpočátku zobrazí v angličtině - pro změnu na jiný jazyk klikněte na **English** v pravé horní části okna.

Jakmile se přihlásíte, můžete kliknout na své uživatelské jméno v horní části stránky. Zde můžete:

- Zobrazte profil Tasking Manager, kde můžete:
    - Aktualizovat svou e-mailovou adresu a odkazy na sociální média
    - Zobrazit svou úroveň zkušenosti s mapováním
    - Vidět seznam a mapu projektů, ke kterým jste přispěli
- Jít na stránku **Zprávy** v nástroji Tasking Manager (to není totéž jako systém zasílání zpráv OpenStreetMap)
- Odhlásit se

### Hledání projektu - Obrazovka Tasking Manageru k zapojení se

Kliknutím na odkaz "Zapojit se" v hlavním menu se dostanete k hlavnímu seznamu projektů v Tasking Manageru.

![TM contribute][]

Strana Tasking Manager Zapojit se je rozdělena do tří hlavních částí:

- možnosti vyhledávání a filtrování vlevo
- Seznam projektů
- Mapové zobrazení seznamu projektů

#### Možnosti hledání a filtrování

Ve výchozím nastavení jsou zobrazeny všechny projekty, které jsou k dispozici pro mapování. Pomocí části Filtry pokročilého vyhledávání na obrazovce můžete dále zúžit projekty, na kterých byste chtěli pracovat.

- Číslo projektu - Pokud znáte číslo projektu, na kterém chcete pracovat, můžete jej zadat a přejít přímo na něj.
- Organizace - umožňuje zobrazit pouze projekty, které byly požadovány jednotlivými organizacemi.
- Obtížnost mapování - Některé projekty je obtížnější mapovat než jiné. Tato možnost vám umožňuje najít projekty, které jsou nejvhodnější pro vaši úroveň zkušeností. Doporučujeme pracovat na projektech, které nejlépe odpovídají vašim zkušenostem, obzvláště pokud jste zkušený mapovač.
- Typ mapování - Umožňuje najít projekty, které obsahují určitý typ objektu, který chcete mapovat. Mnoho projektů je zaměřeno pouze na jeden typ mapování, ale projekty mohou obsahovat více typů úloh, které je třeba mapovat.
- Fulltextové vyhledávání - umožňuje vyhledávat projekty, které mohou obsahovat určité slovo nebo frázi v popisu projektu.
- Značky kampaně - Projekty mohou obsahovat jiné značky, které označují, že větší projekty mapování kampaní jsou součástí projektu, tyto projekty můžete najít zadáním do tohoto pole.

#### Zobrazení mapy
Kliknutím na kartu Zobrazení mapy se zobrazí počet projektů v regionu. Dvojitým kliknutím nebo přiblížením se zobrazí jednotlivé projekty. Jakmile je zvětšeno, body na mapě jsou barevně označeny, červená je naléhavá, žlutá je vysoká nebo střední priorita a šedá je nízká priorita. Kliknutím na některý z bodů na mapě se zobrazí informace o daném projektu. Kliknutím na název projektu se dostanete k tomuto projektu.

![TM project map][]

### Mapování přes Tasking Manager

Jakmile najdete projekt, na kterém chcete pracovat, kliknutím na název projektu se dostanete k podrobnému záznamu pro daný projekt. Tento podrobný náhled obsahuje:

- popis důležitosti projektu a způsob využití dat
- Podrobné pokyny pro to, co mapovat
- výběrové obrazovky pro validaci mapování
- Podrobná mapa oblastí jednotlivých mapovacích úloh s informacemi o jejich stavu.
- Karta Otázky a poznámky k otázkám nebo připomínkám k projektu

![TM project description][]



#### Projektová stránka

Vše, co potřebujete vědět o projektu, je tady! V horní části je úplný popis mapového projektu a informace o projektu.  

Pod popisem je obrazovka rozdělena do levé a pravé části. V levé části je panel se záložkami s kartami pro "Pokyny", "Mapa", "Ověřit" a "Otázky a poznámky". Vpravo je mapa projektu a jednotlivé úkoly pro mapování.

- Neobarvené úkoly jsou připravené a dostupné pro mapování
- Růžové oblasti mapy označují oblasti s vyšší prioritou
- čtverce žluté / zlaté mřížky mají dokončen první průchod mapování a jsou připraveny k ověření (validaci)
- Žlutý rámeček označuje vámi vybraný úkol
- Modré úkoly v současné době mapuje jiný mapovač 
- Zelená úloha byla dokončena 2. průchodem mapování a mapování bylo "ověřeno" (validováno)
- Tmavě šedé úlohy byly mapovány a označeny že nemají přijatelné snímky pro mapování 
- Modrá čára, která je běžně viditelná v obvodových čtvercích projektu, označuje okraj projektu. Tato hranice běžně sleduje dostupné snímky, správní hranici atd., Takže se může zobrazit jako neobvyklý tvar. Přestože mapování může být dokončeno mimo tento okraj, není to požadavek a nebude to považováno od validátorů za nutné.  


#### Karta Pokyny
To ukazuje, co je zapotřebí v mapovací úloze. Projekty se nacházejí v obtížnosti, vhodné pro začátečníky, pokročilé a pokročilé mapovače - a pokyny to vysvětlí. Ujistěte se, že této části po přečtení rozumíte. Existuje mnoho stylů mapového projektu pro mnoho různých účelů. Některé běžné aktivity projektu zahrnují:  

- silniční sítě: používají lidé k nahrání dat do ručních navigačních přístrojů aby s nimi hledali přístup k odlehlým oblastem  
- Mapování vesnic: Často se používá k identifikaci míst, kde lidé žijí a kde mohou být postiženi  
- Mapování budov: Používá se pro posouzení poškození nebo sledování zasažení nemocemi. Používá se také pro odhady počtu obyvatel.  
- Mapování řek, zdí a dalších prvků  

Ne všechny oblasti světa jsou podobné vašim vlastním, takže mohou být poskytnuty konkrétní rady pro značkování. Například africká silniční síť se velmi liší od typických amerických nebo evropských dálnic.  

Zobrazí se oddíl s označením **Změna sady komentářů** Měli byste se ujistit, že se v editačním programu objeví při nahrávání nebo ukládání změn spolu s informacemi **source**, které můžete (v závislosti na vašem editačním softwaru) potřebovat zkopírovat & vložit do zdrojového pole při provádění změn.  

Někdy mohou být k dispozici snímky specifické pro danou úlohu - možná budete muset souhlasit s licencí, abyste získali přístup. Pokyny obvykle označují nejjednodušší způsob, jak je načíst do editorů, jako je JOSM nebo iD.  

Při kontrole úlohy označené jako úplná, ověřovatelé očekávají, že všechny požadavky na kartě s pokyny byly dokončeny. Možná, že dokončení celého úkolu je poměrně obtížné - pokyny uvedené níže jsou k dispozici kolem úloh, které jste odemkli; stejně jako poskytování užitečné zpětné vazby pro další mapovače.  

#### Tlačítko aktivita a statistiky  

Tato záložka obsahuje statistiky o projektu. Je rozdělena na dvě části, podrobný seznam aktivit (dříve na vlastní záložce u Tasking Manager 2.0) a souhrnný oddíl.

The summary contains a list of mappers who have completed at least one task within the project.  

A log of all the comments left on individual tasks is at the bottom of the page. These are comments left on tasks and should not be confused with the "Questions and Comments" tab which are general questions and comments about the overall project.

You can return the main project contribution page by clicking on the project title on the Activity and Stats page.

#### Map Tab  

Click when you are ready to start mapping. You may choose an individual task to work on by selecting it from the map, or by clicking on the "Take a Task at random" option.  Only uncolored tasks can be selected in this tab or you will get a message saying the task can not be mapped. If you intend to validate, make sure you select the "Validate" tab.

![TM map tab][]

#### Výběr úkolu k mapování  

Having selected your task you will be able to see if there is any history for this task, such as a mapper starting to map, but realizing they do not have time to complete the task.  

Clicking on the **Start Mapping** button locks the task so that no other mapper can select it until it is released again, and starts a 2 hour (120 minute) countdown timer, at the end of which time the task is automatically released. It is good practice to check on your countdown timer on a regular basis - it is easy to become engrossed in your mapping and not realise your task has been released, and has now been selected by another mapper who has started mapping it too. This can lead to conflicts and problems.  


#### Editing choices

Different options for editing are presented to you as soon as you lock a task.

##### Editace s JOSM  

Start JOSM before using this link and it will automatically load the existing OSM data into JOSM.  

>  1. 'Enable remote control' needs to be ticked - found under **Edit / Preferences / Remote Control**
>  2. If you have previously installed the plug-in 'continuosDownload' it is best to disable it (untick 'Download OSM Data continuously' under the **File** menu in JOSM).  
>  3. If JOSM does not load the imagery automatically as well, it can normally be found under the **Imagery** menu. [More info on imagery here ](/en/josm/more-about-josm/#add-imagery)  
  

##### iD editor  

Select this to automatically start a new tab or window of your web browser, with existing OSM data loaded. The Internet Explorer web browser does not currently support iD and it will load Potlatch 2 instead. Your original tab or window with the Task Manager will still be present.  


##### Potlatch 2  

The editor will load in a new window or tab. Potlatch will not automatically display the task bounding box, but you can do so by following this procedure:  

1. In the Tasking Manager, select a task and click Start Mapping to lock it  
2. In the Tasking Manager, select Edit with JOSM (if a window appears saying "JOSM remote control did not respond..." just click OK).  
3. Below the Edit with JOSM button, text will say "Tip: Download the following .gpx file...". Download the .gpx file, and note where it is saved.  
4. In the Tasking Manager, change from Edit with JOSM to Edit with Potlatch 2. Potlatch should open in a new tab.  
5. In Potlatch, select Background, then Vector File...  
6. In the Load Vector File window, at the bottom next to File, click Open, and navigate to the .gpx file you just downloaded  
7. In the Load Vector File window, make sure the box is checked in the Show column for the .gpx file, then close the window  
8. Potlatch should now display the boundary as a square (probably cyan). Note that Potlatch will still load data outside the boundary.  
  

##### Field Papers  

For use only when you are involved in a project where a local mapper has carried out a ground survey and marked a printed map with information such as road names. This map can be rescanned and used as a background image for a remote or local mapper to read the information and update the OpenStreeetMap data [Field papers section of LearnOSM](/en/mobile-mapping/field-papers/).  


#### Splitting a task square

Having selected your task and inspected it with the imagery in place, you may realise that there is far too much detail required for mapping. An example of this may be tracing buildings in dense urban areas, or locating small villages in large areas. As guidance, where it isn't possible for one person to complete within the 2 hour time limit you can often split the task into 4 smaller areas. *Use with caution* - if/when task squares are split too small it is difficult to judge what type of highway is involved, and to identify other features.  

> Be aware that other useful comments about the work previously completed will no longer be available.


#### Odemčení úkolu

![TM unlock][]

##### Unlocking a Task before it is complete

If you start working on a task, but cannot complete it for some reason, it is best practice to leave a comment against the task. Simply detail what remains and choose **Stop Mapping**. Make sure your comments are relevant and aimed to help out the next mapper.  

Například:  

    Almost complete, small village top left 
    in the task square to be traced though
  

##### Odemčení úlohy, která je zcela zmapována

It is very difficult to be completely certain that you have completed a task - however it is acceptable to mark the task as complete if you are fairly sure - the contents will be checked by another mapper when validating, and any small additions can be made then.  

For the process to work most effectively, mappers need to mark tasks as "Mapped" rather than leaving them for several other 'not sure' mappers to spend time also checking them.  

When you have finished editing and think that the task is complete, save any remaining edits with your editing programme, then return to the Tasking Manager.  

+ Add comments to the box detailing what you achieved and more importantly, what you are not certain of. For example; "Complete as far as I can see, but there is cloud covering the top right corner of the task & I cannot see to trace this area".  
+ Click on the "Mark as Mapped" button, and your work is ready for review.  

##### Označení úlohy se špatnou fotomapou

You will sometimes select a task that can not be mapped because the imagery is low resolution or has cloud cover. Just close that task in your editor and use the "Mark as Bad Imagery" button to record that the task can not be mapped due to poor imagery.


#### Odeslání zprávy z pole komentáře

When leaving a comment against a task, you can have the comment sent as a message to a named mapper. Much like Twitter, simply use an @ followed by the username. This will send a message to the user containing the comments from this box, plus a link to the task that the comments box relates to.  

Například:  

    @HOTMppr nice work tracing the building  
    details here. You missed a small group  
    of houses on the upper left of the task square,  
    I added a few in, but some still remain.  

This is particularly useful when validating or adding on another's previous work - you can provide feedback, thanks or more.  

+ You may wish to provide a link to a site which may help the mapper, such as <http://learnosm.org/en/coordination/remote-tracing/#buildings-walls-compounds-barriers>  
+ Be aware that many people from around the world will be participating, so prefer simple, clear language. If you come across comments in other languages, tools such as Google Translate are reasonably effective.


#### Referring to a particular task when sending an email  

If you need to send a message, such as an email or an IRC message, and you are querying something concerning a particular task within a project (perhaps you need help identifying something from the satellite imagery):  

1. Click on the task square concerned  
2. Click on the address bar in your web browser, which should show something similar to 'http://tasks.hotosm.org/project/713?task=259'  
3. Copy this link into the message. 


## Získání nápovědy 

### Live text based help

From the Learn page of the Tasking Manager:  
1. Click on **OSM HOT IRC Channel #hot**  
2. Enter a username (your OSM username?), or use the preset characters  
3. At the bottom of the dropdown list select **hot**  

- To the right of the screen is a list of users that are online now.  
- Type your message in the box at the bottom left of the screen (this is sometimes temporarily obscured by other text, but this will disappear as you select the box.  
- To direct a message to a particular individual, include their username from the list on the right within your message. Type, then use the return key to submit your comment. The system is 'live' so wait for an answer - your username will often be used in the reply to show you the comment is directed to you. You will normally receive a reply within a few seconds, so please wait.  
- An alternative simple system can be found at [kiwiIRC.com](https://kiwiirc.com/client/irc.oftc.net/hot)  
- Further info on using IRC with OpenStreetMap may be found at [OSM Wiki IRC](http://wiki.openstreetmap.org/wiki/Irc)  
- Alternatively use an IRC client of your choice (Server=irc.oftc.net, and channel=#hot)  

### Leaving a Project question / comment / contacting the Project creator

Using the "Comments" tab for the project you can see other users' questions and comments and leave one of your own. You can also click the "Contact Project Manager" link and that will automatically direct your comment/question to the project creator. 

All comments are public and it is not real time, live chat, use the IRC option above for realtime chat.

![TM comments][]


## Tipy a triky při editaci  

By now you have a good understanding of what the Tasking Manager is, and some of the various functions it supports. Unlike normal editing, this tool is often used for time critical projects with many participants - this may be a little bit different to what you are used to.  

Some general advice to heed when working in this tool:  

* Avoid mapping far outside of your task square - other mappers may be working in that area, resulting in duplicated efforts. It's OK to map objects such as buildings overlapping a boundary, but avoid going much further - upload immediately after mapping something at the border.  
* Extend roads, streams, or other features slightly over the boundaries - this lets the next mapper pick up where you left off, but upload as soon as you finish editing it.  
* If you are in doubt about what a particular feature is, use the comment section to ask questions or check the wiki.  
* If you make a serious mistake - for example, deleting a major feature or relation - use IRC or the comment box to ask other mappers to help in reverting this for you. Try to include the changeset, or a description of what happened. Being a collaborative task, many other mappers are here to help - it's important to remember everyone makes mistakes sometimes.  
* Don't hesitate to ask for feedback - mappers validating your work can be terse or to the point, but if they know it's OK to engage in a dialog with you, the outcome is often a lot better for all involved. It can be difficult to communicate in another language, and it's easy to appear abrupt when you have to translate as well as pass a message in a language you are not fluent in.  
* You must not validate your own work - a second pair of eyes will always lead to better quality mapping.  
* Don't worry if other mappers are terse when validating your work - like you, they just want to ensure all of the data is mapped accurately. Feedback is invariably about the remaining work, not criticism of your efforts to date.  


## Validace

Validation is the process of a second mapper reviewing the mapping of the initial mapper of a project task. It is designed to ensure complete, quality data and provide thanks, feedback and encouragment to mappers.

### Začínáme

Validation starts much the same way as mapping does, a volunteer finds a project they would like to work on, reads the instructions tab to be sure they understand what is called for and how it is expected to be mapped, but instead of selecting the mapping tab for the project, they select the "Validate" tab.

![TM select for validation][]

The validator can select a task by clicking on an individual task square, clicking "Select a random Task", select by user or draw a polygon to select multiple, connected tasks.

Unlike mappers, validators can select multiple tasks to perform validation on a larger scale than just one task.

### Výběr více úkolů pro validaci

New in the latest version of the Tasking Manager is the ability to select multiple tasks for validation, either by area or by user.

Depending on which editor you are using, this feature will behave differently.

In JOSM, a second OSM data layer will be created titled "Task Boundaries - Do Not Edit or Upload" and it will have uploading disabled in recent versions of JOSM. JOSM **will not download the OSM data** because it could be a very large amount of data. Instead the validator will have to use the task boundaries as a guide and download the data to the active editing layer manually.

#### Select by drawing a polygon

This option allows a validtor to draw a square around a group of tasks and check them all out at once.

Once in the editor of their choice, **the validator will have to manually download the OSM data** for task areas selected. This is to prevent downloading all of the OSM data between the selected Tasks.


#### Select By User

A list of mappers who have marked a task as done is presented. Hovering over anyone in the list will highlight the tasks they have marked as completed. The list also prensents three important pices of information about the mapper, their experience level, the number of days since they first started mapping using the Tasking Manager and the number of days since they last received feedback via validation. This allows the validator to specifically target new mappers, experienced mappers or mappers who have not had any feedback for an extended period of time.

Clicking on the "Start Validating" button will lock all the tasks completed by that mapper and allow the validator to open them in their editor of choice.

![TM multi selection][]

Once in the editor of their choice, **the validator will have to manually download the OSM data** for task areas selected. This is to prevent downloading all of the OSM data between the selected tasks.

### Dokončení validace

Once the validator has finished the validation process either for one task or multiple tasks, they should return to the Tasking Manager and select one of the three choices that reflect the mapping of the task:

- Stop Validating - If you could not complete the validation process but must stop validating.
- Mark (all) as Valid - If the mapping is complete and accurate
- Mark (all) as Invalid - If the mapping is not complete or inaccurate.

For the last two choices the validator can and should leave a friendly, encouraging comment addressed to the mapper(s) involved and provide thanks for their contributions and feedback on their mapping. Please be considerate before marking a task as invalid. If just a few bits are missing add them yourself, explain what was missing in your comment but nevertheless mark the task as valid. New mappers will consider their completed task marked as invalid as a fairly harsh comment.




[TM overview]: /images/coordination/tasking_manager_overview.png
[TM Quick Start 1]: /images/coordination/tasking_manager_qs1.png
[TM Quick Start 2]: /images/coordination/tasking_manager_qs2.png
[TM Quick Start 3]: /images/coordination/tasking_manager_qs3.png
[TM Quick Start 4]: /images/coordination/tasking_manager_qs4.png
[TM Quick Start 5]: /images/coordination/tasking_manager_qs5.png
[TM Quick Start 6]: /images/coordination/tasking_manager_qs6.png
[TM Quick Start 7]: /images/coordination/tasking_manager_qs7.png
[TM Quick Start 8]: /images/coordination/tasking_manager_qs8.png
[TM login 1]: /images/coordination/tasking_manager_login1.png
[TM login 2]: /images/coordination/tasking_manager_login2.png
[TM login 3]: /images/coordination/tasking_manager_login3.png
[TM contribute]: /images/coordination/tasking_manager_contribute.png
[TM map tab]: /images/coordination/tasking_manager_map_tab.png
[TM unlock]: /images/coordination/tasking_manager_unlock_task.png
[TM project map]: /images/coordination/tasking_manager_project_map.png
[TM project description]: /images/coordination/tasking_manager_project_description.png
[TM comments]: /images/coordination/tasking_manager_comments.png
[TM task selection]: /images/coordination/tasking_manager_task_selection.png
[TM select for validation]: /images/coordination/tasking_manager_validation_selection.png
[TM multi selection]: /images/coordination/tasking_manager_multi_selection.png
