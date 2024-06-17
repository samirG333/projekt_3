Projekt 3
projekt_3.py - Projekt tři

Author: Samir Obeidat
Email: samirbdt@gmail.com

Popis
Tento projekt (projekt_3.py) je skript pro web scraping navržený k extrakci a zpracování volebních dat z určených URL adres. Využívá knihovnu requests pro stahování webových stránek a BeautifulSoup pro zpracování HTML obsahu.

Funkce
sestav_url(base_url, relative_url): Funkce pro sestavení kompletní URL adresy z základní URL adresy a relativní URL.
ziskej_nazvy_stran(stranky_url): Získá názvy stran z dané URL adresy pomocí scrapování HTML tabulek.
zpracuj_data(prvni_url, soubor, strany_url): Zpracovává hlavní data z první URL adresy a zapisuje formátovaná data do výstupního souboru.
zpracuj_podrobnosti(druha_url, soubor, radek_data, cislo_radku, seznam_stran): Zpracovává podrobná data z druhé URL adresy a přidává je do výstupního souboru.
hlavni(url, soubor, strany_url): Hlavní funkce pro spuštění zpracování dat.
Použití
Instalace: Ujistěte se, že máte nainstalovaný Python 3.x spolu s potřebnými knihovnami (requests, beautifulsoup4). Můžete je nainstalovat pomocí pip:

Zkopírovat kód
pip install requests beautifulsoup4
Použití z příkazové řádky: Spusťte skript projekt_3.py s požadovanými argumenty:

css
Zkopírovat kód
python projekt_3.py [url] [výstupní_soubor] [url_stran]
url: Adresa URL stránky obsahující volební data.
výstupní_soubor: Název výstupního souboru, do kterého budou uložena zpracovaná data.
url_stran: Adresa URL pro získání názvů stran.
Příklad
Pro spuštění skriptu:

bash
Zkopírovat kód
python projekt_3.py https://example.com/volební_data výstup.csv https://example.com/názvy_stran

