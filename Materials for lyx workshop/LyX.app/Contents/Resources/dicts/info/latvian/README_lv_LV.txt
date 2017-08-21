# Latviešu valodas pareizrakstības pārbaudes bibliotēka (afiksu un vārdnīcas fails) 
# lietošanai ar OpenOffice 2.4.x un augstāk
# Latvian spelling dictionary (affix and dictionary files) for OpenOffice 2.4.x and higher
#
# Copyright (C) 2002-2009 Janis Eisaks, jancs@dv.lv, http://dict.dv.lv
# 
# Šī bibliotēka tiek licencēta ar Lesser General Public Licence (LGPL) 2.1 nosacījumiem. 
# Licences nosacījumi pievienoti failā license.txt vai iegūstami tīmekļa vietnē  
# http://www.fsf.org/licensing/licenses/lgpl.html
# 
# This library is free software; you can redistribute it and/or
# modify it under the terms of the GNU Lesser General Public
# License as published by the Free Software Foundation; either
# version 2.1 of the License, or (at your option) any later version.
#
# This library is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
# Lesser General Public License for more details.
#
# You should have received a copy of the GNU Lesser General Public
# license along with this library; if not, write to the Free Software
# Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA
#

1. Version info
2. Uzstādīšana
3. Interesentiem
4. Izmaiņu saraksts

=================
1. Version info 0.9.0

- izveidots jauns afikss, kas SFX x, kas atbild par sieviešu dzimtes vārdu veidošanu no 
  vīriešu dzimtes vārdiem (skolnieks->skolniece utml);
- attiecīgi mainīta vārdu bāze, pie viena izmetot vairākus gramatiski pareizus, taču idiotiska satura ierakstus;
- papildināts vārdu krājums;

Zināmās problēmas (kā jau parasti):
- iztrūkstoši vārdi vai to atsevišķas formas, kuras lietotāji ir laipni aicināti iesūtīt uz adresi 
  dict@nospam@dv.lv (no adreses jādzēš @nospam) vai, kam būtu dodama priekšroka, 
  ar vietnes http://dict.dv.lv starpniecību darba turpināšanai.

=================

2. Vārdīcas uzstādīšana

Ieteikums: uzstādīt vismaz OO 3.2 versiju.
Izmantojot to, vārdnīcas uzstādīšana ir ļoti vienkārša, izmantojot OO Extension Manager.
Extension Manager piedāvā iespēju kā tiešsaistes tā lokālu paplašinājumu uzstādīšanu.
Ja uzstādīšana tiešsaistes režīmā nav iespējama, vajadzīgo valodas paplašinājumu (vārdnīcu)
var lejupielādēt šeit:

http://extensions.services.openoffice.org/dictionary

un izmantot lokālai uzstādīšanai.

Ja izmantojat OO versiju, kas neuztur Extensions (pirms 2.4.1), tad:

1. iespēja. Uzstādīšana tiešsaistes režīmā
 No izvēlnes File/Wizards/Install new dictionaries palaidiet att. vedni, izvēlieties 
 Jums tīkamo vedņa valodu un sekojiet norādījumiem. Bez latviešu valodas pareizrakstības 
 rīkiem Jūs vienlaicīgi varat uzstādīt papildus valodas vai atsvaidzināt esošās bibliotēkas.
 (Uzmanību! - nav zināms, cik ilgi šī bibliotēka vēl tiks aktualizēta; pilns laidienu arhīvs ir 
  atrodams http://sourceforge.net/projects/openoffice-lv/)

 Ja kaut kādu iemeslu dēļ nevarat izmantot 1. iespēju, ir
 
 2. iespēja. "Offline" uzstādīšana
 Lejupielādējiet pēdējo moduļa versiju no openoffice-lv.sourceforge.net .
 Pēc faila iegūšanas tas ir jāatpako direktorijā %Openoffice%\share\dict\ooo, 
 kur %Openoffice% - direktorija, kurā veikta OpenOffice uzstādīšana. Tur esošajam failam 
 dictionary.lst ir jāpievieno sekojošas rindas: 
 
 DICT lv LV lv_LV
 HYPH lv LV hyph_lv_LV

 vai arī jāizpilda win-lv_LV_add.bat (Windows gadījumā) vai, Linux gdījumā, jāizpilda 
 komandu:

   sh <lin-lv_LV_add.sh

 Lai izpildītu 2. iespēju, Jums ir jābūt tiesībām rakstīt minētajā katalogā. Ja tādu nav, 
 varat uzstādīt vērdnīcu lokāli, savā lietotāja opciju katalogā (%OOopt%/user/wordbook).

 Offline uzstadīšanai var izmantot arī 1. iespējā minēto vedni, viss notiks līdzīgi, 
 tikai nepieciešamajām moduļu pakotnēm būs jābūt uz lokālā diska. Jāpiezīmē ka, piemēram, 
 SUSE gadījumā minētais vednis ir izgriezts ārā no OO un 2. iespeja ir vienīgā. Atsevišķi 
 šis līdzeklis un vārdnīcas ir iegūstams tīmekļa vietnē
 
  http://wiki.services.openoffice.org/wiki/Dictionaries


 Ar to moduļu uzstādīšana praktiski ir pabeigta; atliek vienīgi caur 
 Options>Language settings>Writing aids ieslēgt vai izslēgt nepieciešamos moduļus un 
 iestatīt dokumentu noklusēto valodu.
 

 Ja ir nepieciešama automātiskā pareizrakstības pārbaude, zem Tools>Spellcheck jāieķeksē 
 AutoSpellcheck.
 

3. Interesentiem

Ja jums ir iekrājušies vārdi, kurus šis līdzeklis neatpazīst vai arī atpazīst kļūdaini, esat
laipni aicināti tos atsūtīt tālākai vārdnīcas pilnveidošanai vai arī reģistrēties vārdnīcas 
izstrādei veltītajā vietnē //dict.dv.lv.

Lielāka apjoma dokumentu filtrēšanai var izmantot sekojošā vietā atrodamu StarBasic makrosu:
http://lingucomponent.openoffice.org/servlets/ReadMsg?listName=dev&msgNo=1843

Piezīme - makross nedarbojas ar OO >3.0.

Sarakstu gadījumā ir lūgums sākumā pašiem kritiski izvērtēt neatpazīto vārdu pareizību 
vai to pielietojamību (piem slengs, barbarismi utml. drazas, manuprāt, nav tā vērtas, 
lai tās iekļautu pareizrakstības pārbaudes vārdnīcā, lai gan viena otra tomēr iespraucas).

4. Izmaiņu saraksts
=================
Version info 0.8.1
-lielākas nekā sākotnēji domāts izmaiņas vārdu bāzē;
-aizvāktas dažas atvasinātās vārdu formas, kuras "nenes" pielietojamu jēgu;
=================
Version info 0.8b1
!!! versija uzskatāma par pre-release
-būtiskas izmaiņas aff failā, tālab arī leciens versiju numerācija;
-papildinājumi vārdu bāzē;
-aizvāktas dažas atvasinātās vārdu formas, kuras "nenes" pielietojamu jēgu;
=================
Version info 0.7.4
-labots afiksu fails - kļūdas pēc diviem afiksiem bija vienādas atslēgas (tas
 (laimīgā kārtā, šķiet, neietekmēja vārdnīcas darbaspējas);
-ar roku filtrēti īpašības vārdu krājumi;
-papildināts vārdu krājums
=================
Version info 0.7.3
- labots II deklinācijas afikss (papildināts ar nnis-ņņi)
- būtiski papildināts vārdu krājums;
- novērstas nepilnības vārdu locījumos;
- izķertas dažas kļūdas vārdu krājumā.

Version info 0.7.2
- papildināts vārdu krājums;
- novērstas nepilnības vārdu locījumos
===================

Version info 0.7.1
- korekcijas īpašības vārdu pārāko pakāpju afiksos;
- papildināts vārdu krājums;
- novērstas nepilnības atsevišķu vārdu locījumos
=================
... te dažus ir aizmirsies ierakstīt...
=================
Version info 0.6.4
- būtiskas izmaiņas dažos afiksos, kuru dēļ notika tā, kā notika
- izfiltrēts un pārbaudīts dic fails

=================

Version info 0.6.3c
- daži labojumi aff failā
- papildināts dic fails

=================

Version info 0.6.3a
- izlabots aff fails (neuzmanības kļūda, kas, iespējams, neatstāja ietekmi uz
  darbību
- papildināts dic fails

=================
 
Version info 0.6.3
- izlaboti un optimizēti daži afiksi;
- manuāli izfiltrēts vārdu pamatformu krājums, tuvinot reālai dzīvei;
- koplektā iekļauts arī Jāņa Vilima izstrādātais vārdu pārnesējs v. 0.2 (skat. hyph-lasimani.txt);

Vārdnīcā joprojām iztrūkst šis un tas, tāpēc visi ir mīļi aicināti sūtīt neatpazītos vārdus man (adrese - skat augšā) vai ierosinājumus par pārnesēju - Jānim Vilimam.

Turpmākajos plānos ietilpst vārdnīcas papildināšana un, iespējams, darbības vārdu afiksu pārstrāde, ja eksperimenti apstiprinās aizdomas par kļūdām.

=================
Version info 0.6
- pilnīgi pārveidota afiksu faila struktūra, sadalot locījumus
  pa skaitļiem un pamazināmām formām ar nolūku uzlabot pareizo
  (dzīvē pielietojamo) formu kodēšanu. Ir izdarīti arī vairāki
  afiksu labojumi.


Vārdnīcā 0.6 joprojām nav atrodami:
- darbības vārdi, kuri eksistē tikai refleksīvajās formās
- I konjugācijas darbības vārdu refleksīvās formas
- I konjugācijas darbības vārdu divdabju sufiksi - ošs ošais ams amais
- I konjugācijas darbības vārdu divdabju sufiksi - is dams damais
- lietvārdi-daudzskaitlinieki

Visi, kas lieto šo "brīnumu", ir laipni aicināti sūtīt man neatpazīto
vārdu sarakstus (txt vai swx formātos). 
Visideālākā forma - neatpazītais vārds visos tam raksturīgajos locījumos.

Entuziasti var nodarboties arīdzan ar specializēto vārdnīcu veidošanu, 
kuras var pieslēgt lietošanai OpenOffice paralēli pamatvārdnīcai.

=================
Verson info 0.5.5
- pievienota visa 1. konjugācija....
- lietvārdu pamazināmo formu afiksi

Vārdnīcā 0.5.5 nav atrodami:
- darbības vārdi, kuri eksistē tikai refleksīvajās formās
- lietvārdi-daudzskaitlinieki
- vēl šis un tas

Verson info 0.5sr2
- pievienoti 1. konjugācijas darbības vārdū nākotnes formas

Vārdnīcā 0.5sr2 nav atrodami:
- darbības vārdi, kuri eksistē tikai refleksīvajās formās
- lietvārdi-daudzskaitlinieki
- vēl šis un tas (piem. pamazināmās formas)

Verson info 0.5
- pievienota divdabju veidošana un locīšana
- izlabota kļūda I deklinācijas locīšanā (piem. kuģis)
- izlabota kļūda V deklinācijas locīšanā (piem. roze)
- papildināta vārdnīca (nedaudz)

Vārdnīcā 0.5 nav atrodami:
- 1. konjugācijas darbības vārdi
- darbības vārdi, kuri eksistē tikai refleksīvajās formās
- lietvārdi-daudzskaitlinieki
- vēl šis un tas (piem. pamazināmās formas)

Version info 0.4.1
- izlabots glucks I deklinācijas lietvārdu locīšanā
- pievienoti skaitļa vārdi

Vārdnīcā nav atrodami:
- 1. konjugācijas darbības vārdi
- darbības vārdi, kuri eksistē tikai refleksīvajās formās
- lietvārdi-daudzskaitlinieki
- divdabji, 
- vēl šis un tas


Version info: 0.4
-koriģētas 1. un 4. deklinācija lietvārdu vārdnīcas
-ieviesti afiksi īpašības vārdiem
-pievienoti apstākļa vārdi un īpašības vārdi

Vārdnīcā nav atrodami:
- 1. konjugācijas darbības vārdi
- darbības vārdi, kuri eksistē tikai refleksīvajās formās
- lietvārdi-daudzskaitlinieki
- divdabji, 
- skaitļa vārdi
- vēl šis un tas


Version info: 0.3.1
-izlabots fails .dic, II deklinācijas atslēga (suns, akmens)
-pievienoti 1. un 6. deklinācijas lietvārdi

Vārdnīcā nav atrodami:
- 1. konjugācijas darbības vārdi
- īpašības vārdi, divdabji, apstākļa vārdi, 
- darbības vārdi, kuri eksistē tikai refleksīvajās formās
- skaitļa vārdi
- vēl šis un tas


Version info: 0.3

Vārdnīcā nav atrodami:
- 1. un 6. deklinācijas lietvārdi
- 1. konjugācijas darbības vārdi
- īpašības vārdi, divdabji, apstākļa vārdi, 
- darbības vārdi, kuri eksistē tikai refleksīvajās formās
- skaitļa vārdi
- vēl šis un tas

Version info: 0.3a
izlabots fails .dic, kurā bija zudušas atslēgas IV deklinācijai

Version info: 0.3

Vārdnīcā nav atrodami:
- 1. un 6. deklinācijas lietvārdi
- 1. konjugācijas darbības vārdi
- īpašības vārdi, divdabji, apstākļa vārdi, 
- darbības vārdi, kuri eksistē tikai refleksīvajās formās
- skaitļa vārdi
- vēl šis un tas
