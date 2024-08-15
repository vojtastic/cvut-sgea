---
icon: material/numeric-4-box
title: Cvičení 4
---

# Tvorba webové mapy, export dat

## Cíle cvičení

<div class="grid cards grid_icon_info smaller_padding" markdown> <!-- specificky format gridu (trida "grid_icon_info") na miru uvodni strance predmetu -->

-   :material-map-search-outline:{ .xl }

    vytvoření __interaktivní webové mapy__ s vlastním obsahem

-   :material-chart-box-multiple:{ .xl }

    procvičení jednoduchých __GIS analýz__

-   :material-map-marker-multiple-outline:{ .xl }

    nastavení základní __mapové symbologie__

-   :material-export:{ .xl }

    __export dat__ pro použití v CAD software
</div>

<hr class="level-1">

## Základní topografická mapa a ZABAGED

Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Maecenas porttitor congue massa. Fusce posuere, magna sed pulvinar ultricies, purus lectus malesuada libero, sit amet commodo magna eros quis urna. Nunc viverra imperdiet enim. Fusce est. Vivamus a tellus. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Proin pharetra nonummy pede. Mauris et orci. Aenean nec lorem. In porttitor. Donec laoreet nonummy augue. Suspendisse dui purus, scelerisque at, vulputate vitae, pretium mattis, nunc. Mauris eget neque at sem venenatis eleifend. Ut nonummy.
{style="color:grey;"}

<hr class="level-1">

## Zadání úlohy

Pomocí mapových služeb od ČÚZK vytvořte __webovou mapu__ obsahující budovy (stavební objekty) v zadané obci __barevně rozlišené dle připojení na kanalizaci a plyn__.


<div class="table_centered table_no_padding" markdown>
??? task-fg-color "Individuální zadání"

    | číslo zadání |      jméno      | kód obce |
    | ------------ | --------------- | -------- |
    |   1 |          Abrahámová Anna |  503622  |
    |   2 |            Al Homsi Muaz |  504505  |
    |   3 | Aschenbrennerová Natalie |  505293  |
    |   4 |            Bagirova Sona |  506320  |
    |   5 |         Bártová Kristýna |  507580  |
    |   6 |           Bařinová Adéla |  507717  |
    |   7 |        Bělohradský David |  508152  |
    |   8 |       Belyavskaya Galina |  509647  |
    |   9 |               Beneš Adam |  516619  |
    |  10 |           Beranová Klára |  529575  |
    |  11 |             Berka Matyáš |  529796  |
    |  12 |         Berndtová Eliška |  530115  |
    |  13 |           Bitsman Sofiia |  530298  |
    |  14 |            Bodlák Ondřej |  532011  |
    |  15 |             Bodnar Pavlo |  532142  |
    |  16 |              Boschat Lea |  533017  |
    |  17 |      Bovsunivska Tetiana |  533068  |
    |  18 |          Bunčeková Adéla |  533262  |
    |  19 |        Burešová Michaela |  533271  |
    |  20 |              Buzický Vít |  533424  |
    |  21 |        Candrová Michaela |  533718  |
    |  22 |       Cikánková Karolína |  533831  |
    |  23 |              Danda Tomáš |  533807  |
    |  24 |            Davtyan Davit |  533947  |
    |  25 |      Dlhopolčková Nicole |  534587  |
    |  26 |         Dovhanyčová Nina |  534668  |
    |  27 |         Drajnová Róberta |  534935  |
    |  28 |       Drapáková Kateřina |  535044  |
    |  29 |         Dubrovska Karyna |  535320  |
    |  30 |          Dupčáková Daria |  535338  |
    |  31 |       Durdíková Kateřina |  535931  |
    |  32 |        Durecová Viktória |  536270  |
    |  33 |         Dvořáčková Beata |  537021  |
    |  34 |         Dvořák František |  537225  |
    |  35 |             Edinac Oxana |  537764  |
    |  36 |            Fiala Vojtěch |  538132  |
    |  37 |           Fousková Alice |  539244  |
    |  38 |              Fučík Karel |  539325  |
    |  39 |              Gintner Jan |  539341  |
    |  40 |             Guryča Šimon |  539473  |
    |  41 |           Hájková Eliška |  539660  |
    |  42 |              Haken Tomáš |  540013  |
    |  43 |           Hartová Zuzana |  540196  |
    |  44 |         Havlátová Blanka |  540447  |
    |  45 |         Havlíček Antonín |  540498  |
    |  46 |            Helclová Sára |  540609  |
    |  47 |             Hodek Michal |  540749  |
    |  48 |            Holubec Jakub |  540765  |
    |  49 |             Horák Samuel |  540773  |
    |  50 |          Houžvička Matěj |  540871  |
    |  51 |             Hozlár Matej |  541591  |
    |  52 |            Hvězdová Anna |  541893  |
    |  53 |      Chalupníková Eliška |  542105  |
    |  54 |             Chobot Sláva |  543128  |
    |  55 |          Chuprina Elvira |  544302  |
    |  56 |           Chuprova Elena |  544361  |
    |  57 |         Iakimov Miroslav |  544442  |
    |  58 |        Iefremenko Maryna |  544884  |
    |  59 |            Jágrik Marian |  545007  |
    |  60 |                Janák Jan |  545317  |
    |  61 |                 Jíra Jan |  545414  |
    |  62 |           Kaľavská Petra |  545490  |
    |  63 |       Kalinina Margarita |  545520  |
    |  64 |         Kalousková Adéla |  545597  |
    |  65 |     Karabaeva Anastasiia |  545708  |
    |  66 |           Karlová Simona |  546518  |
    |  67 |              Khalak Yana |  547247  |
    |  68 |          Kiseleva Marina |  547786  |
    |  69 |         Klačanová Monika |  548171  |
    |  70 |             Klapka Lukáš |  548774  |
    |  71 |             Klaus Robert |  548936  |
    |  72 |              Klika Tomáš |  549363  |
    |  73 |      Kocmanová Magdalena |  549380  |
    |  74 |          Kocourek Štěpán |  549860  |
    |  75 |          Kohoutek Ondřej |  550027  |
    |  76 |         Kolková Michaela |  550167  |
    |  77 |        Končelová Marcela |  550353  |
    |  78 |      Körblerová Karolína |  550230  |
    |  79 |               Král Kamil |  550540  |
    |  80 |          Králiková Aneta |  550442  |
    |  81 |            Kreuzová Emma |  550663  |
    |  82 |          Krupička Václav |  550906  |
    |  83 |            Kubias Matouš |  551716  |
    |  84 |              Kušej Pavel |  551791  |
    |  85 |         Kyseľová Martina |  552119  |
    |  86 |          Laibl Christian |  552747  |
    |  87 |       Leissnerová Anežka |  552925  |
    |  88 |          Lekešová Zuzana |  552992  |
    |  89 |              Leník Milan |  553140  |
    |  90 |          Lindaur Vojtěch |  553468  |
    |  91 |       Listíková Michaela |  553794  |
    |  92 |         Listíková Tereza |  554120  |
    |  93 |              Liška Jakub |  554464  |
    |  94 |          Loudová Vendula |  554529  |
    |  95 |         Lysiakova Polina |  554740  |
    |  96 |         Mackovčin Viliam |  555185  |
    |  97 |              Mágrová Eva |  556076  |
    |  98 |           Machů Michaela |  556203  |
    |  99 |             Maléřová Eva |  556718  |
    | 100 |            Maslák Daniel |  556912  |
    | 101 |             Mikuda Tomáš |  557005  |
    | 102 |     Mlynárová Anna-Marie |  557013  |
    | 103 |          Molinková Karin |  558303  |
    | 104 |     Morgensternová Lucie |  558371  |
    | 105 |                Muk Filip |  559237  |
    | 106 |         Němcová Karolína |  559806  |
    | 107 |         Němečková Eliška |  560057  |
    | 108 |        Neveršilová Klára |  560359  |
    | 109 |          Neznamova Nelli |  560570  |
    | 110 |      Nguyenová Quynh Hoa |  561398  |
    | 111 |            Nikolaev Oleg |  561681  |
    | 112 |             Novák Martin |  561967  |
    | 113 |        Nováková Kateřina |  562751  |
    | 114 |           Novotná Tereza |  562882  |
    | 115 |           Padevět Štěpán |  564133  |
    | 116 |            Páleník Filip |  563226  |
    | 117 |         Panznerová Lucie |  563382  |
    | 118 |           Pekárek Martin |  563811  |
    | 119 |         Peukertova Aneta |  563919  |
    | 120 |           Pham Son Duong |  564184  |
    | 121 |           Picková Tereza |  564231  |
    | 122 |          Plášilová Julie |  565164  |
    | 123 |         Pokorná Kateřina |  565792  |
    | 124 |          Pořízková Klára |  566004  |
    | 125 |           Prášková Klára |  566241  |
    | 126 |           Prášková Marie |  566306  |
    | 127 |         Procházka Martin |  566578  |
    | 128 |       Procházková Monika |  566900  |
    | 129 |             Přibyl Matěj |  567167  |
    | 130 |       Reicheltová Sabina |  567612  |
    | 131 |             Rydval Tomáš |  567698  |
    | 132 |         Rychlíková Marie |  568007  |
    | 133 |              Říha Martin |  569160  |
    | 134 |           Saitzová Julie |  569585  |
    | 135 |              Saxová Anna |  569666  |
    | 136 |             Sazima Lukáš |  569691  |
    | 137 |       Selnekovičová Anna |  569917  |
    | 138 |            Sgibneva Lada |  571491  |
    | 139 |       Shkrabo Anastasiia |  572462  |
    | 140 |             Sloupová Eva |  572829  |
    | 141 |         Smutková Barbora |  572926  |
    | 142 |             Socha Ondřej |  573299  |
    | 143 |           Součková Julia |  573493  |
    | 144 |       Stejskalová Tereza |  573825  |
    | 145 |        Střihavková Lucie |  573990  |
    | 146 |               Suchá Anna |  574015  |
    | 147 |             Suprun Alisa |  574058  |
    | 148 |            Sychrová Anna |  574082  |
    | 149 |               Šich Tomáš |  574210  |
    | 150 |        Šmejkal Jan Jakub |  574767  |
    | 151 |              Šmida Filip |  574899  |
    | 152 |           Štefko Nicolas |  574988  |
    | 153 |        Tenglerová Tereza |  576131  |
    | 154 |              Teplý Filip |  576247  |
    | 155 |        Terekhova Tetiana |  576336  |
    | 156 |            Tomková Aneta |  576590  |
    | 157 |               Touš Lukáš |  576808  |
    | 158 |            Trnková Lucie |  576883  |
    | 159 |           Trojáček Lukáš |  577162  |
    | 160 |           Trousil Matyáš |  577197  |
    | 161 |       Tsaizel Anastasiia |  578134  |
    | 162 |           Typlová Tereza |  578282  |
    | 163 |          Uherková Tereza |  578355  |
    | 164 |        Vaculová Gabriela |  578428  |
    | 165 |              Vajc Daniel |  579432  |
    | 166 |           Valenta Tadeáš |  579777  |
    | 167 |         Vaňková Viktorie |  579874  |
    | 168 |              Vavra Jakub |  580147  |
    | 169 |      Velichinskaia Daria |  580651  |
    | 170 |          Vojtěchová Anna |  581178  |
    | 171 |            Vokatý Martin |  581259  |
    | 172 |             Volfová Jana |  581879  |
    | 173 |          Vopalecká Lucie |  582239  |
    | 174 |         Vůchová Veronika |  582859  |
    | 175 |    Zakaurtseva Ekaterina |  584045  |
    | 176 |           Zemanová Aneta |  584631  |
    | 177 |             Zonyga Šimon |  584983  |
</div>

## Pracovní postup

<div class="annotate" markdown>

- Do prázdné mapy v ArcGIS Online __přidejte vrstvu__ __:material-layers: RÚIAN__{.bg}, __podvrstvu__ __:material-layers-triple: Obec__{.bg} z [__Geoportálu ČÚZK__](https://geoportal.cuzk.cz/ "Služby → Prohlížecí → Esri ArcGIS Server (nebo WMS)"){.color_def .underlined_dotted .external_link_icon target="_blank"}. Tato vrstva obsahuje polygony území všech obcí v ČR.__(1)__{title="ukázka"}

- Vrstvě __nastavte :material-filter: filtr dle kódu__ (v krajním případě dle názvu) __zadané obce__. Filtr omezí zobrazení prvků pouze na jednu zadanou obec.__(2)__{title="ukázka"}

- Do mapy dále __přidejte vrstvu__ __:material-layers: RÚIAN__{.bg}, __podvrstvu__ __:material-layers-triple: StavebniObjekt__{.bg} z [__Geoportálu ČÚZK__](https://geoportal.cuzk.cz/ "Služby → Prohlížecí → Esri ArcGIS Server (nebo WMS)"){.color_def .underlined_dotted .external_link_icon target="_blank"}. Tato vrstva obsahuje polygony všech stavebních objektů v ČR.__(3)__{title="ukázka"}

- __Prostorovou analýzou__ (nástroj __:material-tools: Overlay Layers__{.bg}) __vytvořte vrstvu stavebních objektů pouze na území zadané obce__.__(4)__{title="nastavení parametrů nástroje"}__(5)__{title="ukázka výsledku"}

    - nastavte mapové okno tak, aby byla __viditelná celá hranice zadané obce__ a *parametr __"Processing Extent"__ nastavte na __"Display Extent"__*{.primary_color .no-dec} (parametr omezí výpočet na rozsah mapového okna, výrazně se tím sníží cena výpočtu)

- Pomocí stylů __nastavte budovám symbologii dle atributu "Připojení na kanalizační síť"__. Kategorie typu "nedefinováno", "nezjištěno" apod. __musí mít nastavenou neutrální šedou barvu__ (dle kartografických zvyklostí). Barvy výplně zvolte dle citu, volitelně přidejte i barevné ohraničení.__(6)__{title="ukázka"}

- Vrstvu duplikujte a nově vytvořené kopii __nastavte symbologii dle atributu "Připojení na rozvod plynu"__. V seznamu vrstev __změňte číselné kategorie na slovní popisy__{.primary_color} dle následujícího klíče:

<div class="table_centered table_no_padding grid" style="margin:0px;" markdown> <!-- https://squidfunk.github.io/mkdocs-material/reference/grids/#using-generic-grids -->

<div markdown>

__:material-pipe: Připojení na kanalizační síť__
{align="center" style="margin:0px;"}

|KÓD| NÁZEV                     |
|---|---------------------------|
| 1 | Přípoj na kanalizační síť |
| 2 | Vlastní ČOV               |
| 3 | Žumpa, jímka, septik      |
| 4 | Bez kanalizace a jímky    |
| 8 | Nedefinováno              |
| 9 | Nezjištěno                |

</div>
<div markdown>

__:material-gas-burner: Připojení na rozvod plynu__
{align="center" style="margin:0px;"}

|KÓD| NÁZEV                |
|---|----------------------|
| 1 |Plyn z veřejné sítě   |
| 2 |Plyn z dom. zásobníku |
| 3 |Bez plynu             |
| 8 |Nedefinováno          |
| 9 |Nezjištěno            |
| 51|Plyn v domě           |

</div>
</div>

- Přidejte __Základní topografickou mapu (S-JTSK)__ od ČÚZK či __ortofoto (S-JTSK)__ od ČÚZK __jako podkladovou mapu__.__(7)__{title="ukázka"}

    - Aby se vrstva přidala jako podkladová mapa (Basemap), je nutné ji přidat tlačítkem __:material-button-cursor: Použít jako podkladovou mapu__{.bg} (Use a basemap)
    - Nastavením podkladové mapy v systému JTSK dojde ke správnému zarovnání budov s podkladovou mapou.

<!-- NEFUNGUJE MI TA ZMENA PROJEKCE, U TETO VRSTVY TO TREBA FUNGUJE: geoappext.nrcan.gc.ca/arcgis/rest/services/BaseMaps/CBMT3978/MapServer -->

- Vrstvám s klasifikací budov __nastavte exkluzivní viditelnost__{.underlined_dotted title="funguje pouze na seskupené vrstvy"}, aby byla při přepínání viditelná vždy pouze jedna z nich. Ostatní vrstvy z mapy odstraňte.__(8)__{title="ukázka"}

- __Webovou mapu uložte__ s názvem "Jmeno_Prijmeni_SGEA2025" a __nastavte sdílení v rámci oganizace__{.primary_color} nebo __veřejné__{.primary_color}.

- Vyučujícímu odevzdejte __URL adresu webové mapy__.__(9)__

???+ task-fg-color "Výsledek (část první): Webová mapa"

    <iframe width="100%" height="400" frameborder="0" scrolling="no" marginheight="0" marginwidth="0" src="https://experience.arcgis.com/experience/0e6a7769af1d479489af74e2f98ca195"></iframe>


<!--

![](https://dummyimage.com/600x400/0065bd/57b1ff&text=v%C3%BDsledn%C3%A1+webov%C3%A1+mapa){width=500px}
{align=center}
<figcaption>ukázka správného výsledku (webová mapa)</figcaption>

-->


---

- Obě vrstvy (stavební objekty i obvod zadané obce) __exportujte do formátu Shapefile__ a __stáhněte na disk počítače__.

- Shapefile __konvertujte do formátu DXF__. Použijte například [tento](https://mygeodata.cloud/converter/shp-to-dxf){.color_def .underlined_dotted .external_link_icon target="_blank"} webový nástroj.

- Konvertovaný soubor otevřete v CAD software a __vytvořte jednoduchý výkres__ obsahující pouze __obvod zadané obce__ a (jinou barvou) __obvody stavebních objektů__ v ní. Všechny objekty musí být ve formě linií. Výkres odevzdejte ve formátu PDF.

???+ task-fg-color "Výsledek (část druhá): Výkres"

    <iframe src="https://drive.google.com/file/d/1MSAjhVjESNXBqnbiRNS2tz16X78QGy1Q/preview" width="100%" height="400" style="border:0;"></iframe>

- Pomocí :simple-arcgis: ArcGIS Pro (desktopová verze platformy ArcGIS, mimo rozsah kurzu) lze CAD výkres generovat s rozlišením vrstev dle atributu (tedy například rozlišit stavební objekty dle připojení na kanalizační síť i v CAd výkresu)
<!--

![](https://dummyimage.com/600x400/0065bd/57b1ff&text=výsledný+CAD+výkres){width=500px}
{align=center}
<figcaption>ukázka správného výsledku (CAD výkres)</figcaption>

-->

</div> <!-- pro anotace -->

1.  ![](../assets/cviceni04/img01.png){ .no-filter width=700px} vrstva "RÚIAN/Obec"
2.  ![](../assets/cviceni04/img02.png){ .no-filter width=700px} filtr dle kódu obce
3.  ![](../assets/cviceni04/img03.png){ .no-filter width=700px} vrstva "RÚIAN/StavebniObjekt"
4.  ![](../assets/cviceni04/img04.png){ .no-filter width=200px}<br> parametry nástroje "Overlay Layers"
5.  ![](../assets/cviceni04/img05.png){ .no-filter width=700px} výsledná vrstva (budovy jsou pouze uvnitř hraice obce)
6.  ![](../assets/cviceni04/img06.png){ .no-filter width=700px} změna symbologie (barva výplně a obrysu)
7.  ![](../assets/cviceni04/img07.png){ .no-filter width=700px} změna podkladové mapy (Základní topografická mapa)
8.  ![](../assets/cviceni04/img08.png){ .no-filter width=700px} exkluzivní viditelnost skupiny vrstev v legendě
9.  __Příklad odevzdaného odkazu:__<br>https://ctuprague.maps.arcgis.com/apps/mapviewer/index.html?webmap=21df15ae2ca9458794a16a8fd9078b78


<hr class="level-1">

## Odevzdání

Povinnými výstupy úlohy jsou __webová mapa__ a __CAD výkres__. Webová mapa je po uložení a nastavení sdílení přístupná přes __URL adresu__, kterou je nutné odevzdat vyučujícímu. Spolu s CAD výkresem ve formátu DWG je tyto výstupy __nutné odevzdat přes systém Moodle__.

Úloha je uznána, pokud webová mapa a CAD výkres obsahují __všechny požadované náležitosti__ (viz níže).

???+ note-grey "Požadované náležitosti odevzdaných výstupů"
    __Webová mapa__

    - vrstva se stavebními objekty __omezena hranicí obce__, naopak žádné __stavební objekty nesmí chybět__
    - __legenda se slovními popisy__ (nikoli s číselnými kódy)
    - kategorie typu "nedefinováno", "nezjištěno" apod. neutrální __šedou barvou__
    - podkladová mapa – __Základní topografická mapa__ nebo __Ortofoto od Zeměměřického úřadu__
    - na vrstvy rozlišující připojení na kanalizaci a plyn nastavená __exkluzivní viditelnost__ (nesmí být možné je zobrazit současně)
    - sdílení webové mapy nastaveno __"v rámci organizace"__ či __"veřejně"__, __bez správného sdílení k mapě nemá vyučující přístup a nedojde ke kontrole__{style="color:#c22521;" .icon-exclm .no-dec}

    __CAD výkres__

    - __formát PDF__
    - obsahem musí být __pouze hranice obce__ a __stavební objekty__ (omezené hranicí obce)
    - hranice obce __barevně odlišena__ od stavebních objektů
    - __název obce__ stejnou barvou jako hranice obce

### Opravy

V případě, že odevzdaný výstup není správný, je vyučujícím emailem __vrácen k opravě__. Opravený výstup se odevzdává opět prostřednictvím systému Moodle. Výstup lze odevzdat po __maximálně dvou opravách__, v případě pozdního odevzdání či nesprávného výstupu po druhé opravě je úloha __trvale označena jako nesplněná__.

[Tabulka hodnocení úloh](../hodnoceni.md){ .md-button .md-button--primary }
{align=center}

<br><br><br><br><br>


<style>
    .underlined_dotted {border-bottom: .05rem dotted var(--md-default-fg-color--light);}
    .color_def {color:var(--md-default-fg-color) !important;}
    .no-wrap {white-space: nowrap;}
    .bg {border-radius: .1rem;  background-color: var(--md-default-fg-color--lightest);  padding:.1em .4em; white-space: nowrap;}
</style>