# AC - Implementační báze - Nápověda

Tento repozitár slouží k evidenci nápovědy D365 Business Central 

## Obsah nápovědy

Pro psaní nápovědy k addonům dodržujte náležitosti:
 - Název souboru nápovědy se bude skládat z:
   - ```ac-nazevpacku-nazevsouboru.md```
   - *(```ac-pp-helpdesk.md```)*
 - Pro každý addon vzniknou dva soubory, jeden pro popis a použití, druhý pro nastavení.
   - Například: ```ac-pp-helpdesk.md``` a ```ac-pp-helpdesk-setup.md```
 - Struktura souborů nápovědy je:
   - Nadpis, krátký popis a kroky jak danou činnosti udělat.
   - viz. vzorová nápověda [Helpedsku](business-central/AC-IB/ac-pp-helpdesk.md)
 - ### Vlastnosti a tagy
    Každý dokumentu musí obsahovat hlavičku v následujícím tvaru

    ```
    ---
    title: Czech Local Functionality - Advance payments and invoices | Microsoft Docs
    description: This section describes local functionality - Advance payments and invoices
    author: ac-kunes
    ms.service: dynamics365-business-central
    ms.topic: article
    ms.devlang: na
    ms.tgt_pltfrm: na
    ms.workload: na
    ms.search.keywords: Czech, Advance payment, Advance invoices, Payables, Finance, CZ, Cash
    ms.date: 15/05/2019
    ms.author: v-pejano
    ---
    ```
- Každý dokument musí nakonci obsahovat tabulku "Viz také"

    Pod každým souborem nápovědy bude odkaz na nadřazený balík a také odkaz na nastavení daného addonu nebo v opačném případě na obecný popis s návodem k použitíí.


    Příklad konce souboru HelpDesk (použití):


```
## Viz také
[HelpDeks - Nastavení](business-central/AC-IB/ac-pp-helpdesk-setup.md)  
[AC Productivity pack](business-central/AC-IB/ac-pp-productivity-pack.md)
```

- Pro základní editaci je zde [šablona](template.md).



## Pojmenovávání souborů

### Pravidla
- Nenechávat mezery mezi slovy v názvu souboru, používejte pomlčky.
- Používejte pouze malá písmena.
- Limit je maximálně 80 symbolů.
- Všechny soubory musí být ve formátu markdown (.md).



## Nahrávání souboru
Při každém nahrávání, editaci nebo mazání souborů je nutné podepsat každý **commit** svým jménem a popsat o jako událost se jedná.

  ### Commit Changes

  *Martin Kuneš - Náhrání nových úprava stávajících souborů*

  *Přidány nové soubory nápovědy a aktualizace dle legislativy*.

## Struktura souborů repoziáře

Ujistěte se, že se nacházíte ve správné větvi.
  - Soubory ukládejte do **master Branche**

Soubory standardní nápovědy nahrávejte do:
 - business-central/...
 - *business-central/get-started.md*

Soubory pro addony nahrávejte do:

 - business-central/nazev-slozky-baliku/
 - *business-central/AC-IB/ac-pp-productivity-pack.md*

## Základní syntaxe

### Obecný text

Text není třeba formátovat. Pro tučné písmo slouží dvě hvězdičky, pro kurzívu jedna. Mezi odstavci a nadpisy musí být volný řádek. Pro text na další řádek, je za větou třeba napsat dvě mezery (V případě enteru, text nezačíná na novém řádku).

```
*Kurzíva*
**Tučný text**
***Tučně a kurzíva***


# Téma

## Nadpis 1

Vzorový text, vzorový text, vzorový text, vzorový text, vzorový text, vzorový text, vzorový text.
```

### Nadpisy

Pro nadpisy slouží symbol dvojítého křížku. Dle počtu křížků se rozlišuji úrovně nadpisů. 

```
# Hlavní nadpis
## Název kapitoly
### Název podkapitoly
```


### Odrážky a seznamy

Odrážky pomocí pomlčky

  ```
  - odrážka 1
  - odrážka 2
  ```
### Číslovaný seznam

Stačí psát pouze číslo a tečku.

```
1. Položka
2. Položka
```

### Odkaz na jiný soubor

V hranatých závorkách je text, který se zobrazí a v závorce název souboru. (V tomto případě je soubor finance ve stejné složce.)

```
[Finance](finance.md)
```