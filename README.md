
DOKUMENTĀCIJA PROJEKTAM “LĀČPLĒSIS — ANIMĒTS DIGITĀLAIS EPOSS”

1. Projekta pārskats

Šis projekts ir interaktīva tīmekļa lapa, kas veltīta latviešu eposam “Lāčplēsis”. Projekta galvenais mērķis ir apvienot literāro saturu ar modernām tīmekļa tehnoloģijām, izveidojot vizuāli pievilcīgu un animētu lietotāja pieredzi.

Lapa satur:
- navigācijas izvēlni,
- parallaksa efektu,
- animācijas skrollēšanas laikā,
- informācijas sadaļas par eposu,
- interaktīvu faktu sistēmu,
- adaptīvu dizainu mobilajām ierīcēm.

Projektā izmantotas HTML5, CSS3 un JavaScript tehnoloģijas.


2. HTML dokumenta struktūra

HTML dokuments sākas ar <!DOCTYPE html>, kas norāda, ka tiek izmantots HTML5 standarts. Tālāk tiek definēts <html lang="lv">, kas nosaka lapas valodu kā latviešu.

Dokuments sastāv no divām galvenajām daļām:
- <head> — konfigurācijas un stilu sadaļa,
- <body> — redzamais lapas saturs.

Head sadaļā tiek definēta:
- simbolu kodēšana UTF-8,
- mobilajām ierīcēm pielāgota viewport konfigurācija,
- lapas nosaukums,
- CSS stili.

Body sadaļā atrodas visa lietotāja redzamā informācija.


3. Navigācijas sistēma

Navigācijas josla atrodas lapas augšdaļā un ir fiksēta (position: fixed), tādēļ tā paliek redzama arī skrollējot lapu.

Navigācijā ir četras saites:
- Sākums,
- Eposs,
- Tēli,
- Autors.

Katrs navigācijas elements izmanto enkura saites (href="#id"), kas ļauj ātri pāriet uz konkrētu sadaļu lapā.

Navigācijas dizains ietver:
- caurspīdīgu fonu,
- blur efektu,
- hover animācijas,
- apakšējās līnijas efektu uzbraucot ar peli.

Kad lapa tiek ielādēta, navigācija parādās ar animāciju slideDown.


4. Hero sekcija

Hero sekcija ir pirmā vizuālā sadaļa lapā. Tā satur lielu attēlu ar Latvijas mežu tematiku.

Šajā sadaļā tiek izmantots:
- liels fona attēls,
- parallaksa efekts,
- absolūtā pozicionēšana.

Parallaksa efekts tiek realizēts ar JavaScript palīdzību. Skrollējot lapu, attēls pārvietojas lēnāk nekā pārējais saturs, radot dziļuma iespaidu.

Hero sekcija arī palīdz radīt emocionālu un atmosfērisku ievadu projektam.


5. Eposa informācijas sadaļa

Sadaļā “Lāčplēsis” tiek aprakstīts:
- eposa vēsturiskais konteksts,
- nozīme latviešu kultūrā,
- saikne ar nacionālo identitāti,
- vēsturisko notikumu un folkloras apvienojums.

Šī sadaļa izmanto:
- centrētu virsrakstu,
- baltu informācijas bloku,
- ēnu efektus,
- hover animāciju.

Hover laikā informācijas bloks nedaudz paceļas uz augšu, izmantojot CSS transformācijas.


6. Varoņu sadaļa

Varoņu sadaļā tiek attēloti galvenie eposa tēli:
- Lāčplēsis,
- Laimdota,
- Kangars,
- Spīdala.

Tēli tiek izvietoti CSS Grid režģī ar divām kolonnām.

Katram tēlam ir:
- nosaukums,
- apraksts,
- hover efekts.

Kad lietotājs uzbrauc ar peli uz tēla bloka:
- parādās kreisā robeža,
- mainās fona krāsa,
- palielinās atkāpe.

Tas rada modernu interaktivitātes efektu.


7. Autora sadaļa

Autora sadaļa satur informāciju par Andreju Pumpuru.

Tiek aprakstīts:
- autora dzīves periods,
- viņa ieguldījums latviešu literatūrā,
- folkloras materiālu vākšana,
- eposa radīšanas mērķis.

Sadaļas dizains ir līdzīgs pārējām informācijas kartēm, lai saglabātu vienotu vizuālo stilu.


8. Interaktīvo faktu sistēma

Lapas apakšdaļā atrodas interaktīvā sadaļa “Zināšanu krātuve”.

Tajā ir:
- teksta lauks,
- poga “Atklāt faktu”.

Kad lietotājs nospiež pogu:
1. JavaScript izvēlas nejaušu faktu no masīva,
2. esošais teksts kļūst caurspīdīgs,
3. tiek ielādēts jauns fakts,
4. teksts atkal parādās.

Tas rada dinamisku un interaktīvu lietotāja pieredzi.


9. CSS dizaina sistēma

Projektā tiek izmantoti CSS mainīgie (:root), kas ļauj centralizēti pārvaldīt dizaina krāsas.

Definētās krāsas:
- akcenta krāsa,
- fona krāsa,
- teksta krāsa,
- robežu krāsa.

Tas uzlabo:
- koda pārskatāmību,
- dizaina konsekvenci,
- vieglāku tēmu maiņu nākotnē.


10. Animācijas

Projektā tiek izmantotas vairākas CSS animācijas.

SlideDown:
Animācija tiek izmantota navigācijas parādīšanai no augšas.

FadeInUp:
Animācija paredzēta elementu parādīšanai no apakšas.

Reveal sistēma:
Elementi sākotnēji ir paslēpti un kļūst redzami, kad tie nonāk lietotāja ekrānā.

Šī sistēma tiek realizēta ar:
- CSS klasēm,
- IntersectionObserver API.


11. JavaScript funkcionalitāte

Projektā JavaScript nodrošina trīs galvenās funkcijas.

Parallaksa efekts:
Skrollējot lapu, hero attēls pārvietojas ar citu ātrumu nekā saturs.

Scroll Reveal:
Elementi kļūst redzami, kad lietotājs tos ieskrollē redzamajā zonā.

Nejaušo faktu sistēma:
Pogas nospiešana ģenerē nejaušu faktu no sagatavota masīva.

JavaScript kods ir organizēts vienkārši un saprotami, izmantojot modernās pārlūku API.


12. Responsīvais dizains

Projektā izmantots @media noteikums mobilajām ierīcēm.

Kad ekrāna platums ir mazāks par 768 pikseļiem:
- varoņu režģis pāriet vienā kolonnā,
- samazinās virsrakstu izmēri,
- saturs kļūst ērtāk lasāms telefonos.

Tas nodrošina labu lietotāja pieredzi dažādās ierīcēs.


13. Projekta stiprās puses

Projektam ir vairākas priekšrocības:
- moderns dizains,
- gludas animācijas,
- vienkārša navigācija,
- responsivitāte,
- kultūras tematika,
- laba vizuālā struktūra,
- interaktivitāte bez ārējām bibliotēkām.


14. Iespējamie uzlabojumi

Nākotnē projektā varētu pievienot:
- tumšo režīmu,
- audio efektus,
- animētus SVG elementus,
- datubāzi ar faktiem,
- daudzvalodu sistēmu,
- smooth scrolling,
- dinamisku satura ielādi.


15. Secinājums

Šis projekts ir veiksmīgs piemērs modernai front-end izstrādei, kur kultūras saturs tiek apvienots ar interaktīvām tīmekļa tehnoloģijām.

Tiek demonstrētas:
- HTML struktūras prasmes,
- CSS animācijas,
- adaptīvais dizains,
- JavaScript interaktivitāte.

Projekts ir piemērots:
- izglītības platformām,
- kultūras projektiem,
- studentu darbiem,
- front-end portfolio demonstrācijai.
