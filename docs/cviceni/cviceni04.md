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


<hr class="level-1">

## Zadání úlohy

Pomocí mapových služeb od ČÚZK vytvořte __webovou mapu__ obsahující budovy (stavební objekty) v zadané obci __barevně rozlišené dle připojení na kanalizaci a plyn__.

## Pracovní postup

Do prázdné mapy v ArcGIS Online přidejte vrstvu "RÚIAN" z [__Geoportálu ČÚZK__](https://geoportal.cuzk.cz/ "Služby → Prohlížecí → Esri ArcGIS Server (nebo WMS)"){.color_def .underlined_dotted .external_link_icon target="_blank"}, podvrstvu "Obec". Tato vrstva obsahuje polygony území všech obcí v ČR.

Na vrstvu obcí nastavte filtr dle názvu (nebo lépe dle kódu) zadané obce. Filtr omezí zobrazení prvků pouze na jednu zadanou obec.

Do mapy dále přidejte opět vrstvu "RÚIAN" z [__Geoportálu ČÚZK__](https://geoportal.cuzk.cz/ "Služby → Prohlížecí → Esri ArcGIS Server (nebo WMS)"){.color_def .underlined_dotted .external_link_icon target="_blank"}, tentokrát podvrstvu "StavebniObjekt". Tato vrstva obsahuje polygony všech stavebních objektů v ČR.

Překryvnou analýzou (nástroj Overlay Layers) vytvořte vrstvu stavebních objektů pouze na území zadané obce.

Pomocí stylů nastavte budovám symbologii dle atributu "Připojení na kanalizační síť". Kategorie typu "nedefinováno", "nezjištěno" apod. musí mít nastavenou neutrální šedou barvu (dle kartografických zvyklostí).

Vrstvu duplikujte a nově vytvořené kopii nastavte symbologii dle atributu "Připojení na rozvod plynu".

V seznamu vrstev změňte číselné kategorie na slovní popisy dle následujícího klíče:

<div class="table_centered table_no_padding" markdown>

__Kanalizace__
{align="center"}

|KÓD| NÁZEV                     |
|---|---------------------------|
| 1 | Přípoj na kanalizační síť |
| 2 | Vlastní ČOV               |
| 3 | Žumpa, jímka, septik      |
| 4 | Bez kanalizace a jímky    |
| 8 | Nedefinováno              |
| 9 | Nezjištěno                |

__Plyn__
{align="center"}

|KÓD| NÁZEV                |
|---|----------------------|
| 1 |Plyn z veřejné sítě   |
| 2 |Plyn z dom. zásobníku |
| 3 |Bez plynu             |
| 8 |Nedefinováno          |
| 9 |Nezjištěno            |
| 51|Plyn v domě           |

</div>

Obě vrstvy (stavební objekty i obvod zadané obce) exportujte do formátu Shapefile a stáhněte na disk počítače.

Shapefile konvertujte do formátu DXF.

Výsledný soubor otevřete v CADu a vytvořte jednoduchý výkres obsahující obvod zadané obce a (jinou barvou) stavební objekty v ní. Výkres odevzdejte ve formátu PDF.

Webové mapě nastavte radio button k přepínání vrstev kanalizace a plynu, ostatní vrstvy odstraňte.

Přidejte podkladovou mapu Základní topografickou mapu od ČÚZK či ortofoto.

Webové mapě nastavte sdílení v rámci organizace či veřejné.

Webovou mapu uložte a její odkaz odevzdejte.


## Odevzdání






<style>
    .underlined_dotted {border-bottom: .05rem dotted var(--md-default-fg-color--light);}
    .color_def {color:var(--md-default-fg-color) !important;}
    .no-wrap {white-space: nowrap;}
    .bg {border-radius: .1rem;  background-color: var(--md-default-fg-color--lightest);  padding:.1em .4em; white-space: nowrap;}
</style>