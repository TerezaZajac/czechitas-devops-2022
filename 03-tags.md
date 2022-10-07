### K čemu v Gitu slouží značky (tzv. „tagy“)?
Slouží především ke značení důležitých míst v historii. Nejčastěji se používá u jednotlivých vydání.


### Jak lze značky vytvořit?
anotované značky:
$ git tag -a v1.4

prosté značky:
$ git tag v1.4


### Jak vypsat jejich seznam?
Pro výpis všech dostupných: 
$ git tag

pro konkretní serii:
$ git tag -l "v1.8.5*"


### Jak je smazat?
$ git tag -d <tag_name>


### Můžete ke značce připojit i komentář nebo delší popis? Jak?
Ano, u anotovaných, buď parametrem -m nebo Git spustí textový editor, v němž zprávu zadáte.
