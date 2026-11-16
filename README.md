# Szakdolgozat kódok és adatbázisok - Konrád Ábel Sámuel
Ez a repozitórium a szakdolgozatomhoz készült empirikus kutatás  - nyelvi modellek antiszemitizmus-vizsgálata -  
Python kódjait és elemzéseit tartalmazza
## A repozitórium fájljai:
Pilot fázis kódjai:
   **Pilot_n720_adatbázis_futtato.ipynb**
    * **Leírás:** A 720 elemű pilot kutatás adatgyűjtését végző szkript. Lekérdezi a válaszokat a megjelölt nyelvi modellektől, rögzíti a tokenstatisztikákat, és elmenti az eredményeket.
   **Pilot_Claude_kódolás_humán_kódolás.ipynb**
    * **Leírás:** A pilot adatok gépi (Claude Sonnet) annotálásának, a kódolói megbízhatóság (intra-rater és inter-rater reliability / Cohen-kappa) tesztelésének, valamint a validációs minták előállításának kódja.
Éles kutatás küdjai
   **Szakdolgozat_kódja_fin.ipynb**
     **Leírás:** A teljes, 4800 elemű fő kutatási adatbázis generálásának, a Claude általi többségi gépi kódolásának és a statisztikai modelleknek a futtatókódja.

## Használati útmutató
A notebookok futtatásához szükséges API-kulcsokat biztonsági okokból elmaszkoltam a kódban 
így saját kulcsokkal lehet őket reprodukálni.
A notebookookat a fenn látott sorrendben szükséges lefuttatni.
A futások 2026 október 26. és november 6. között folytak - az utolsó simítások a szakdolgozat beadásának napján, november 16-án történtek.

## Csomagok és szoftververzió
*   **Programozási nyelv:** Python 3.13.2 (ipykernel)
  * **Adatkezelés és  számítások:**
    * pandas – Adatbázisok étrehozása, szűrése, összefésülése és mentése
    * numpy – Numerikus tömbök, mátrixműveletek és matematikai függvények
  * **Statisztika, modellezés és értékelés:**
    * statsmodels (statsmodels.miscmodels.ordinal_model.OrderedModel)
    * scipy (scipy.stats, scipy.optimize, scipy.special) 
    * sklearn (sklearn.metrics.cohen_kappa_score, accuracy_score, confusion_matrix)
    * patsy – 
* ** API kliensek és kérések:**
  * openai – OpenAI API kliens (GPT modellek hívásához és Batch API-hoz)
  * google-genai (google.genai, google.genai.types) – Google Gemini API kliens 
  * anthropic – Anthropic API kliens 
  * requests – HTTP kérések kezelése
* **Fájlformátumok kezelése:**
  * `openpyxl` – Excel fájlok  olvasása és írása
  * 
