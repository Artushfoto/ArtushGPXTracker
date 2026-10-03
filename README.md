# Artush GPX Tracker 📱📍

**Lehký, jednoúčelový a bezreklamní Android GPS logger navržený pro fotografy.**

Artush GPX Tracker slouží k přímému a přesnému záznamu GPS tras v čase **UTC**. Je vytvořen jako ideální mobilní společník pro párování zeměpisných souřadnic k fotografiím v aplikaci **ArtushVision AI** i v jakémkoliv jiném foto editoru s podporou GPX geotaggingu.

---

## 🌟 Hlavní výhody a vlastnosti

* **Přísné UTC časové razítko (ISO-8601):** Všechny body jsou ukládány v čistém satelitním UTC čase bez časových posunů nebo letního/zimního času.
* **Záznam i při stání na místě (`minDistance = 0 m`):** Aplikace neztrácí body, ani když fotograf stojí delší dobu na jednom místě (např. na vyhlídce či v ateliéru).
* **Ukládání do SQLite databáze (Room):** Každá souřadnice je okamžitě zapsána do paměti. Ani při vybití baterie nebo restartu telefonu nepřijdete o zaznamenaná data.
* **Plně responzivní rozvržení pro všechny telefony:** Písmo a velikosti prvků se automaticky přizpůsobí displeji tak, aby ovládací prvky byly vždy vidět bez nutnosti skrolovat.
* **Historie a správce tras („Moje trasy“):** Přehledný archiv všech vašich výprav. Trasy lze přejmenovávat, přidávat k nim poznámky, zobrazovat v mapách nebo mazat.
* **Chytré zobrazení na mapě:** Přímá integrace s **Mapy.cz**, **Google Earth** nebo Google Maps. Pokud v mobilu chybí GPX prohlížeč, aplikace nabídne odkazy na Google Play a záložní zobrazení polohy.
* **Synchronizace času fotoaparátu („Hodiny“):** Obrazovka s velkým časem a milisekundami. Stačí ji vyfotit fotoaparátem před/během focení a v **ArtushVision AI** zapsat zobrazený čas pro bleskové spárování.
* **Dvoujazyčné rozhraní (English / Čeština):** Snadné přepínání jazyka i intervalu nahrávání (1s až 1min) přímo v nastavení.

---

## 🧭 Popis prvků a ovládání aplikace

Aplikace obsahuje 4 přehledné záložky v dolní navigační liště:

### 1. Záznam (`Record`)
* **Stav sledování (HUD karta):**
  * **Služba:** Zobrazuje, zda záznam běží (`SLUŽBA AKTIVNÍ` / `SLUŽBA ZASTAVENA`).
  * **Start & Trvání:** Zobrazuje čas spuštění záznamu v UTC a živé počítadlo doby trvání.
  * **Stav polohy:** Bleskový přehled o kvalitě GPS fixu (🟢 Kvalitní, 🟠 Použitelný, 🔴 Výpadek).
  * **Telemetrie:** Zobrazuje stáří posledního bodu, přesnost v metrech (Accuracy), nadmořskou výšku a celkový počet zaznamenaných bodů.
* **Tlačítka akcií:**
  * **[Zobrazit polohu v mapě]:** Otevře Google Maps se špendlíkem na vaší aktuální pozici.
  * **[▶ START ZÁZNAMU / ■ STOP ZÁZNAMU]:** Spustí nebo zastaví nahrávání trasy na pozadí. Při novém startu se aplikace zeptá, zda chcete pokračovat v rozepsané trase, nebo začít novou.
  * **[Mapa]:** Otevře celou vykreslenou GPX trasu v aplikaci Mapy.cz nebo Google Earth.
  * **[Sdílet]:** Bleskové odeslání GPX souboru do PC (Quick Share, e-mail, Google Disk).

### 2. Moje trasy (`Tracks`)
* Kompletní historie všech uložených výprav.
* U každé trasy vidíte název, datum, čas od–do a počet bodů.
* **Možnosti úprav:**
  * ✏️ **Přejmenovat trasu** (např. *Křivoklátsko - podzimní focení*).
  * 📝 **Přidat poznámku / popis**.
  * 🗺️ **Prohlédnout v mapové aplikaci**.
  * 📤 **Sdílet GPX**.
  * 🗑️ **Smazat trasu z paměti**.

### 3. Hodiny (`Clock`)
* Černé AMOLED pozadí s velkým lokálním i UTC časem včetně milisekund.
* Vyfoťte tuto obrazovku fotoaparátem před nebo během focení. V **ArtushVision AI** pak v kalkulátoru jednoduše opíšete zobrazený čas pro okamžité časové spárování fotek s GPX trasou.

### 4. Nastavení (`Settings`)
* **Interval obnovování polohy:** Volba frekvence záznamu od 1 sekundy (vysoká přesnost) až po 1 minutu (úspora baterie).
* **Jazyk aplikace:** Přepínání mezi Angličtinou a Češtinou.
* **Odkazy a informace:** Přímé odkazy na stažení mobilního trackeru i desktopového programu **ArtushVision AI**.

---

## 📷 Využití pro geokódování a párování fotek

Vygenerované `.gpx` soubory jsou v přísně standardním formátu **GPX 1.1** a lze je použít v jakémkoliv programu pro geokódování fotografií:

### 1. ArtushVision AI (Doporučeno) 💻
[ArtushVision AI](https://vision.artushfoto.eu) je pokročilý desktopový program pro automatické generování popisků, inteligentní správu klíčových slov a bleskové párování GPS tras z tohoto trackeru:
* Využívá vyfotografovanou obrazovku **Hodiny** pro automatický výpočet časového posunu fotoaparátu.
* Zapisuje přesné GPS souřadnice přímo do EXIF/XMP metadat fotografií.

### 2. Adobe Lightroom Classic
* V modulu **Map (Mapa)** zvolte *Tracklog ➔ Load Tracklog...* a vyberte soubor vyexportovaný z Artush Trackeru.
* Lightroom automaticky rozmístí vaše fotografie na mapu podle EXIF časů.

### 3. Zoner Photo Studio X
* V modulu **Správce** vyberte fotky a zvolte *Mapa ➔ Přiřadit GPS ze souboru GPX...*.

### 4. Další kompatibilní programy
* **GeoSetter**, **Darktable**, **DigiKam**, **Apple Photos** a jakýkoliv jiný software podporující GPX 1.1.

---

## 🌐 Odkazy a stažení

* **Mobilní aplikace Artush GPX Tracker:** [https://tracker.artushfoto.eu](https://tracker.artushfoto.eu)
* **Desktopový software ArtushVision AI:** [https://vision.artushfoto.eu](https://vision.artushfoto.eu)
