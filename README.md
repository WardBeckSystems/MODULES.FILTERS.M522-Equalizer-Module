# M522 Equalizer Module · Filters

Ward-Beck Systems M522, 1986|19. Wiki page: [M522 on WBSps.ca](https://wardbecksystems.github.io/WBSps.ca/PAGES/M522.html)

| Folder | What is in it | Files |
|---|---|---|
| [SCHEMATICS/](SCHEMATICS/) | electrical drawings: schematics, functional diagrams, component layouts, wiring | 75 |
| [MECHANICAL/](MECHANICAL/) | front panels, cover plates, metalwork, assemblies; the front panel as vectors | 20 |
| [PINOUTS/](PINOUTS/) | the RTO-144 connector: connection sheets, connector layouts, rear views | 8 |
| [MANUALS/](MANUALS/) | manuals, manual pages, price lists, brochures, documents | 253 |
| [PHOTOS/](PHOTOS/) | photographs of the module | 22 |
| [SOFTWARE/](SOFTWARE/) | program listings, firmware, the plugin | 1 |
| [KICAD/](KICAD/) | KiCad schematics traced from the drawings, the symbol, PCB projects | 22 |
| [OCR/](OCR/) | the note of every file: date, origin, title block, OCR text | 90 |

<!-- module data: tools/module_specs.py, tools/forum_quotes.py -->

**On the WBSps forum (2006|39 - 2014|47):** [11 topics](FORUM.md): what owners and technicians said about it.

## Specifications

From the technical data sheet: [19xx - M522 - 522A - P003 - 1-1.jpg](MANUALS/19xx%20-%20M522%20-%20522A%20-%20P003%20-%201-1.jpg) page 1 (read by OCR; check against the page). As data: [`Specifications.json`](Specifications.json).

| | |
|---|---|
| **Gain** | Unity +/-0.25 dB |
| **Frequency response** | +/-0.5 dB from Hz kHz with the equalizer inserted and cut/boost controls the detent position |
| **Noise** | dBm absolute (20 Hz cut/boost controls the kHz / equalizer detent position |
| **Harmonic distortion** | Less than from 20 Hz kHz +20 dBm output level less. Less than 0.01% at kHz +20 dBm output level |
| **Source impedance** | Less than ohms unbalanced |
| **Input impedance** | Greater than 4K ohms unbalanced |
| **Input level** | 6dBm nominal +20 dBm maximum |
| **Output impedance** | Less than ohms unbalanced |
| **Load impedance** | SK ohms greater |
| **Output level** | dBm nominal +22 dBm maximum. |
| **Channel separation** | Phasing: Greater than Input and output are phase with the equa izing controls the detent position |
| **Equalization tracking** | Within 0.5 dB |
| **Power requirements** | +/-25 volts dc (M522 40 ma), (M522A 65 ma) |
| **Ambient temperature** | 60 degrees Celsius |
| **Dimensions** | 60&quot; wide 7.00&quot; high 50&quot; deep (41 mm 178 mm 165 mm) |
| **Weight** | M522 M522A (0.485 kg) net. (0.565 kg_ net |

## Circuit description

From [19xx - M522 - 522A - Equalizer (2).pdf](MANUALS/19xx%20-%20M522%20-%20522A%20-%20Equalizer%20(2).pdf) pages 7-12 (read by OCR; check against the pages). As data: [`CircuitDescription.json`](CircuitDescription.json).

<details><summary>Read it</summary>

The left channel 01 Ihe MS2 2A Siereo Equalizer will be described. This i s the same CirCuit r y thai applies tot he M522 Mono Equalizer.

The unbalanced audio input appears at pin 4 o f the module connector. It is r o ul e d dIrectly to the normally closed con ta&lt;:1 of Equalizer Inserts witch SW2A and 10 buffer amplifier UI B.

Mid - Fr e q u e n c y Equalizer

The output from the input buffer a mpli f le r UIB feedS s u mm, n g amptifier U I A and the Mid-F requ ency cu t/boosl control R4. R4 bridges between t n e input and OUlput of summing amplifier U I A.

The arm of R4 conneclS the signal tot h e Slate v &quot;ri&quot;ble filler UJA, UJ8, and U4A. C6 through C9 along wi lh RIS and R18 determine there Son a n l frequency oft h eli l le r.

1'l8 adjusts the ov erail fIller gain and therefore its Q. High Q is nominally four and Low Q is nom in&quot;l ly two.

The filler oUl pu l is fed ba&lt;: k into summing amplifier UI A via CS. This feedback s 1g n a l adds or sub l ra c ts from the mains i g ned in p roporation to its magnitude and p h &quot; sere lat ions hip.

Low Frequency Equalizer

The output from U t A feeds Ih e audios igna l to Ihe low frequen&lt;:y summing amplifier U2B.

Low Frequency CUI/ boost con l r o l R 23 bridges across U2B, wi lh thea r m of this con l r o l coupling the audios i g n alt h rough C II to Low-p &quot; ss filter U4B. The f r e q u e n &lt;:y determining &lt;:ompo nen l S of Ihis filter are theLF shelf contro! R27, R29, C l 2and C lJ.

The filter output is fed b,,&quot;,ck to summing amplifier U28 through R30. Dependenl upon Ihe selling o f c u t/boos l con l rol R2 3 the signal is

added Or sub l r acted from the main signal path thus &quot;Hee ling the

frequency response che r-a c t er-istlc s of the Low Frequency port ion o f

the audios p e c t rum.

**CIRCUIT OESCR IPT ION**

High F r eq u e n c y Equali:&gt;:ation

The summing ampl ifi &quot;r U2A forms the high frequency equal i&gt;:er section, &quot;lo ng with cu t/boost control R34 and a high pass filter made u p of U5 and its associated components.

U2A mixes the main paths i g na l (through R33) and the feedback signal (through R38) to affect the frequency res pon seef the high frequency portion of the audio spectrum from 3.7 kHz up to 15 kHz.

The error or feedback signal is coupled tot he high pass fl lt&quot;r through C1 5. The frequency determining components of this filter are the HF shelf control R4 3, R4 2, cIa and C 19.

The output from thee qua liz e r circu il ry is coupled through C20 to the normally open sec l lon of SW2A, Ih e insertions &quot;, itch. The unbalanced audio &quot;,-, tpu t appears atp in 6 of Ihe module edge con neClor.

Power Supply

The +1-25 volt po &quot;,,,r supply vol lage is decoup Ied via the series type decouplers 01 through 0 4. Divider ne lwork RS6, RS7 and RS9 set I he decoupl er output vol lage t o +1_ 18 volts.

**FREQUENCY RESPONSE CHARACTERISTICS**

5 1==;::::=

3 1--

**I-- &lt;, 1--**

3 I--1

• I--1---9 I--1--

**I-- I-- ~**

t::= t::::: t:: ~

**HIGH FREQUENCY SECTION**

BOOST/ CUT: 1 15 ea FREQUENCY, 3.7_ kHz to 15 kHz

**FREQUENCY RESPONSE CHARACTERISTICS**

9 r---

-15

**100H, == ==**

&quot;'&quot; 10k 2a&lt;.30k4Ok

**MID FREO UE NCY SECT ION**

BOOST/C UT: t I S dB FREQUENCY: 400 Hz to 6.4 ~H..

**FREQUENCY RESPONSE CHA,RACTERIST ICS**

MS22!M S22A. EQUAL l Z ER MODULE

**LOW FREQUENCY SECTION**

BOOST /C UT: tIS d B se -a, T O~200_ H z

**FREQUENCY:**

= ' -.!!!C&quot;&quot;-'=!!!C- -''''''-__---'MFG PAAT NUMBER cr Capae 'lor 4.1 u F/ to V TJ9OBH5 MOI QAS C2 JJ uF /10 V TJ900ll6MOl OA.S ca 4.7 uF /to V Tl 906475M010AS ce 4.1 uF / to V cs 10uF/'15V

e 6)

cal 8000 pF 5' CQ92_MC_l00-802M

COl 8000 pF 5' ere 68 uF /6 V Philips 122$3689

cn 4.1 uF /l0 V TJ 90B475 M010A.S

O. 02 2uF 0.047 u F 68 u F/6 V 5',_.

PhilipS

**CQ92MC-100-223M**

CQ'J2_MC_ l 00-473M 12253689 COS I u F/J5 V T39OB1Q5MOJ 5AS 680 pF Philips 2222_6 30_0368 1 2 20 pF 2222_630-00 221 2100 pF CQ92MC_l00-272M 1500 pF CQ92-MC_100-152M l ]uF/l0V TJ 900 l 36MOIOA.S

Capacllor 0.1 uF/ IOO V Spra gu e I C 1OX7R104M0506 22 uF/25 V Philips 426ET F22 22 uF/25 V 22 u F/25 V 22 uF /2 5 V

e.. 22 u F/ 25 V

22 uF/ 25 V

0.1 u F/ I OO V Sp r ague

0.1 uF/ I OO V

</details>

<!-- /module data -->

## Photos

_Photographs of the module itself: front, back, inside, racked._

<table>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKWW5MY2YxOEt1Y00/view?resourcekey=0-9ZgYWWEK2Gs_m46QeJA0Ew" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKWW5MY2YxOEt1Y00&resourcekey=0-9ZgYWWEK2Gs_m46QeJA0Ew" width="240" alt="19xx - M522 - Equalizer 2.jpg"></a><br><sub>19xx - M522 - Equalizer 2</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKTGJDR3M4cFFHcVk/view?resourcekey=0-xYC2ZazHiwn3UUPLAQ9ZPw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKTGJDR3M4cFFHcVk&resourcekey=0-xYC2ZazHiwn3UUPLAQ9ZPw" width="240" alt="19xx - M522 - Equalizer.jpg"></a><br><sub>19xx - M522 - Equalizer</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKMTRraXpZbk1jYjQ/view?resourcekey=0-FNVXjmiMG8jSrgsykoZ8ag" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKMTRraXpZbk1jYjQ&resourcekey=0-FNVXjmiMG8jSrgsykoZ8ag" width="240" alt="19xx - M522 - IMG_3486.jpg"></a><br><sub>19xx - M522 - IMG_3486</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKMV83QlVSMzRUWEE/view?resourcekey=0-0eHEzH09zRpQUB74x2MinA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKMV83QlVSMzRUWEE&resourcekey=0-0eHEzH09zRpQUB74x2MinA" width="240" alt="19xx - M522 - IMG_3490.jpg"></a><br><sub>19xx - M522 - IMG_3490</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKcWhNQVhMQUQ0OVE/view?resourcekey=0-3C9VYmOaKHGcAai8P_zrKQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKcWhNQVhMQUQ0OVE&resourcekey=0-3C9VYmOaKHGcAai8P_zrKQ" width="240" alt="19xx - M522 - IMG_3493.jpg"></a><br><sub>19xx - M522 - IMG_3493</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKb2VuWTlJY1ctaHc/view?resourcekey=0-nmmoHZ_9HcF6D8mYRTqO8g" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKb2VuWTlJY1ctaHc&resourcekey=0-nmmoHZ_9HcF6D8mYRTqO8g" width="240" alt="19xx - M522 - IMG_3497.jpg"></a><br><sub>19xx - M522 - IMG_3497</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKZ2hKSmVMcDJJSE0/view?resourcekey=0-1dfK6m_3v9-2_OUIYdp-Hw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKZ2hKSmVMcDJJSE0&resourcekey=0-1dfK6m_3v9-2_OUIYdp-Hw" width="240" alt="19xx - M522 - IMG_3499.jpg"></a><br><sub>19xx - M522 - IMG_3499</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKLUxhSFZ6RjUtaTg/view?resourcekey=0-IDluux8zPDa9Y5I1lIivgw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKLUxhSFZ6RjUtaTg&resourcekey=0-IDluux8zPDa9Y5I1lIivgw" width="240" alt="19xx - M522 - Input Module 2.jpg"></a><br><sub>19xx - M522 - Input Module 2</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKOE1KT2xxUThOZGM/view?resourcekey=0-u1x-G2vI58AgXE3RfJdAlg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKOE1KT2xxUThOZGM&resourcekey=0-u1x-G2vI58AgXE3RfJdAlg" width="240" alt="19xx - M522 - Input Module 3.jpg"></a><br><sub>19xx - M522 - Input Module 3</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKWm9sMUVZY1NpWTA/view?resourcekey=0-V196Go-g_ApdINFt3S5z9Q" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKWm9sMUVZY1NpWTA&resourcekey=0-V196Go-g_ApdINFt3S5z9Q" width="240" alt="19xx - M522 - Input Module.jpg"></a><br><sub>19xx - M522 - Input Module</sub></td></tr>
</table>

Not on Google Drive yet: `19xx - M522 - #EQ #Photos-l1600-1.jpg`, `19xx - M522 - #EQ #Photos-l1600-2.jpg`, `19xx - M522 - #EQ #Photos-l1600-3.jpg`, `19xx - M522 - #EQ #Photos-l1600-4.jpg`, `19xx - M522 - #EQ #Photos-l1600-5.jpg`, `19xx - M522 - #EQ #Photos-l1600-6.jpg`, `19xx - M522 - #EQ #Photos-l1600-7.jpg`, `19xx - M522 - #EQ #Photos-l1600.jpg`

## Mechanical

_Mechanical drawings: front panels, cover plates, metalwork and hardware (-03- drawings), AutoCAD files, each with its `(EXTRACTED).svg` vectors; `<module> - front panel.svg` is the front panel as vectors._

<table>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKd0dnX0hUc3FSdzQ/view?resourcekey=0-xc_Min6i5z9s-N4arNA_lw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKd0dnX0hUc3FSdzQ&resourcekey=0-xc_Min6i5z9s-N4arNA_lw" width="240" alt="19xx - M522 - 522-04-001 - EQUALIZER MODULES MODULE LAYOUT.jpg"></a><br><sub>19xx - M522 - 522-04-001 - EQUALIZER MODULES MODULE LAYOUT · <a href="MECHANICAL/19xx%20-%20M522%20-%20522-04-001%20-%20EQUALIZER%20MODULES%20MODULE%20LAYOUT%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKR3ZsaDhPTjlwMkU/view?resourcekey=0-gqkJgSzkMRI7piBUi5JKZQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKR3ZsaDhPTjlwMkU&resourcekey=0-gqkJgSzkMRI7piBUi5JKZQ" width="240" alt="19xx - M522 - 522-04-001 - NQTE NOT SUPPL IED.jpg"></a><br><sub>19xx - M522 - 522-04-001 - NQTE NOT SUPPL IED · <a href="MECHANICAL/19xx%20-%20M522%20-%20522-04-001%20-%20NQTE%20NOT%20SUPPL%20IED%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKY1BkakNsd3JZNVU/view?resourcekey=0-8S-UUmyhXYLRW_EeyyBZ6g" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKY1BkakNsd3JZNVU&resourcekey=0-8S-UUmyhXYLRW_EeyyBZ6g" width="240" alt="19xx - M522 - DOC - 3642-04-003 - ADERS STEREO MASTER FADERS MONO INPUT FADERS.jpg"></a><br><sub>19xx - M522 - DOC - 3642-04-003 - ADERS STEREO MASTER FADERS MONO INPUT FADERS · <a href="MECHANICAL/19xx%20-%20M522%20-%20DOC%20-%203642-04-003%20-%20ADERS%20STEREO%20MASTER%20FADERS%20MONO%20INPUT%20FADERS%20(EXTRACTED).svg">vectors</a></sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKenNPSW1LTXUxSFE/view?resourcekey=0-zhyTu4D10huQ3fzzJgta2g" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKenNPSW1LTXUxSFE&resourcekey=0-zhyTu4D10huQ3fzzJgta2g" width="240" alt="19xx - M522 - DOC - 522-04-001 - FRONT PANEL LAYOU.jpg"></a><br><sub>19xx - M522 - DOC - 522-04-001 - FRONT PANEL LAYOU · <a href="MECHANICAL/19xx%20-%20M522%20-%20DOC%20-%20522-04-001%20-%20FRONT%20PANEL%20LAYOU%20(EXTRACTED).svg">vectors</a></sub></td></tr>
</table>

## Schematics

_Electrical drawings: schematics (-02-), functional diagrams (-01-), component layouts (-06-), wiring (-09-), PCB files (.pcb .dsn), and beside each scan its `(EXTRACTED).svg`: the vectors traced from it._

<table>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKWHBvaUs3SF9lYU0/view?resourcekey=0--2xbl8CeWrE2_sp16Y2y3g" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKWHBvaUs3SF9lYU0&resourcekey=0--2xbl8CeWrE2_sp16Y2y3g" width="240" alt="19xx - M522 - 522-01-001 - EQUALIZER MODULE FUNCTIONAL.jpg"></a><br><sub>19xx - M522 - 522-01-001 - EQUALIZER MODULE FUNCTIONAL · <a href="SCHEMATICS/19xx%20-%20M522%20-%20522-01-001%20-%20EQUALIZER%20MODULE%20FUNCTIONAL%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKelNwbFNNOEs3RmM/view?resourcekey=0-Km30KeVK1sbopLKSUih6aQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKelNwbFNNOEs3RmM&resourcekey=0-Km30KeVK1sbopLKSUih6aQ" width="240" alt="19xx - M522 - 522-01-001.jpg"></a><br><sub>19xx - M522 - 522-01-001 · <a href="SCHEMATICS/19xx%20-%20M522%20-%20522-01-001%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKOVJpSFVVX3RJM00/view?resourcekey=0-ow8bnOJqBeIstm2_6hHV0A" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKOVJpSFVVX3RJM00&resourcekey=0-ow8bnOJqBeIstm2_6hHV0A" width="240" alt="19xx - M522 - 522-01-002 - EQUALIZER MODULE FUNC TIONAL.jpg"></a><br><sub>19xx - M522 - 522-01-002 - EQUALIZER MODULE FUNC TIONAL · <a href="SCHEMATICS/19xx%20-%20M522%20-%20522-01-002%20-%20EQUALIZER%20MODULE%20FUNC%20TIONAL%20(EXTRACTED).svg">vectors</a></sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKc2o1SWVJano4U2s/view?resourcekey=0-oL_wXXbYMTFnZ9haYnHTqQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKc2o1SWVJano4U2s&resourcekey=0-oL_wXXbYMTFnZ9haYnHTqQ" width="240" alt="19xx - M522 - 522-01-002.jpg"></a><br><sub>19xx - M522 - 522-01-002 · <a href="SCHEMATICS/19xx%20-%20M522%20-%20522-01-002%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKbGFNYnlKMm1SOU0/view?resourcekey=0-YFsg7pguyTzlSxuaihpknQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKbGFNYnlKMm1SOU0&resourcekey=0-YFsg7pguyTzlSxuaihpknQ" width="240" alt="19xx - M522 - 522-02-001 - UNLESS OTHERWISE SPECIFIED COM LAST COMPONENT DESIGNAT IONS.jpg"></a><br><sub>19xx - M522 - 522-02-001 - UNLESS OTHERWISE SPECIFIED COM LAST COMPONENT DESIGNAT IONS · <a href="SCHEMATICS/19xx%20-%20M522%20-%20522-02-001%20-%20UNLESS%20OTHERWISE%20SPECIFIED%20COM%20LAST%20COMPONENT%20DESIGNAT%20IONS%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKWTRGamc3NGlOYlk/view?resourcekey=0-El1vDhYmcQE9w2ZK3dbTEQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKWTRGamc3NGlOYlk&resourcekey=0-El1vDhYmcQE9w2ZK3dbTEQ" width="240" alt="19xx - M522 - 522-02-001 - WUKS ALL CAPACITORS ARE.jpg"></a><br><sub>19xx - M522 - 522-02-001 - WUKS ALL CAPACITORS ARE · <a href="SCHEMATICS/19xx%20-%20M522%20-%20522-02-001%20-%20WUKS%20ALL%20CAPACITORS%20ARE%20(EXTRACTED).svg">vectors</a></sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKSlVzR2I0UU1tbWs/view?resourcekey=0-5A7jqbSM6XhE_4RuhvGvlw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKSlVzR2I0UU1tbWs&resourcekey=0-5A7jqbSM6XhE_4RuhvGvlw" width="240" alt="19xx - M522 - 522-02-002 - ALL CAPACITORS ARE UNLESS OTHERWISE SPEC.jpg"></a><br><sub>19xx - M522 - 522-02-002 - ALL CAPACITORS ARE UNLESS OTHERWISE SPEC · <a href="SCHEMATICS/19xx%20-%20M522%20-%20522-02-002%20-%20ALL%20CAPACITORS%20ARE%20UNLESS%20OTHERWISE%20SPEC%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKRHhMb3VWWERtaE0/view?resourcekey=0-IyCyhBiDNvBFfK_6PvEztQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKRHhMb3VWWERtaE0&resourcekey=0-IyCyhBiDNvBFfK_6PvEztQ" width="240" alt="19xx - M522 - 522-06-001 - EQUALIZER MODULE COMPONENT LAYOUT.jpg"></a><br><sub>19xx - M522 - 522-06-001 - EQUALIZER MODULE COMPONENT LAYOUT · <a href="SCHEMATICS/19xx%20-%20M522%20-%20522-06-001%20-%20EQUALIZER%20MODULE%20COMPONENT%20LAYOUT%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKd1Nic3ZLMDRNbUk/view?resourcekey=0-PbUAYZx49sJVFyVQ8NwSCA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKd1Nic3ZLMDRNbUk&resourcekey=0-PbUAYZx49sJVFyVQ8NwSCA" width="240" alt="19xx - M522 - 522-06-002 - EQUALIZER MODULE COMPONENT LAYOUT.jpg"></a><br><sub>19xx - M522 - 522-06-002 - EQUALIZER MODULE COMPONENT LAYOUT · <a href="SCHEMATICS/19xx%20-%20M522%20-%20522-06-002%20-%20EQUALIZER%20MODULE%20COMPONENT%20LAYOUT%20(EXTRACTED).svg">vectors</a></sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKRFhMS0kzOVFva1U/view?resourcekey=0-iru-eFc-A_vl2ZrI3aQliQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKRFhMS0kzOVFva1U&resourcekey=0-iru-eFc-A_vl2ZrI3aQliQ" width="240" alt="19xx - M522 - A B - P19 - Filter Schematic.jpg"></a><br><sub>19xx - M522 - A B - P19 - Filter Schematic · <a href="SCHEMATICS/19xx%20-%20M522%20-%20A%20B%20-%20P19%20-%20Filter%20Schematic%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKT3NBRlh5MTlOTDg/view?resourcekey=0-35TtBaz8as-yDxXaTPQcfg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKT3NBRlh5MTlOTDg&resourcekey=0-35TtBaz8as-yDxXaTPQcfg" width="240" alt="19xx - M522 - A B - P21 - Filter Component Layout.jpg"></a><br><sub>19xx - M522 - A B - P21 - Filter Component Layout · <a href="SCHEMATICS/19xx%20-%20M522%20-%20A%20B%20-%20P21%20-%20Filter%20Component%20Layout%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKNE5TcDJMSVF6ZW8/view?resourcekey=0-zvTSsHCGN8wYSSWEpLNBuQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKNE5TcDJMSVF6ZW8&resourcekey=0-zvTSsHCGN8wYSSWEpLNBuQ" width="240" alt="19xx - M522 - A B - P22 - Component Layout.jpg"></a><br><sub>19xx - M522 - A B - P22 - Component Layout · <a href="SCHEMATICS/19xx%20-%20M522%20-%20A%20B%20-%20P22%20-%20Component%20Layout%20(EXTRACTED).svg">vectors</a></sub></td></tr>
</table>

Not on Google Drive yet: `19xx - 522-01-001 - EQUALIZER MODULE FUNCTIONAL - ISS 1.jpg`, `19xx - 522-01-002 - EQUALIZER MODULE FUNCTIONAL - ISS 1.jpg`, `19xx - 522-02-001 - EQUALIZER MODULE SCHEMATIC - ISS 3.jpg`, `19xx - 522-02-002 - EQUALIZER MODULE SCHEMATIC - ISS 3.jpg`, `19xx - 522-02-003 - MONO EQUALIZER MODULE SCHEMATIC - ISS 1.jpg`

## Pinouts

_Pinouts: the RTO-144 edge connector (connection sheets, connector layouts and rear views, strapping), and the pinout / connections drawings made from them. The module root `RTO.json` lists every contact._

<table>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKX3RqRnJXRzF5VGM/view?resourcekey=0-ImElcit3UxQFUSQunl-rag" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKX3RqRnJXRzF5VGM&resourcekey=0-ImElcit3UxQFUSQunl-rag" width="240" alt="19xx - M522 - A B - P14 - Pinouts.jpg"></a><br><sub>19xx - M522 - A B - P14 - Pinouts · <a href="PINOUTS/19xx%20-%20M522%20-%20A%20B%20-%20P14%20-%20Pinouts%20(EXTRACTED).svg">vectors</a></sub></td></tr>
</table>

## RTO-144 pinout

25 contacts, 2 contacts (P1). Read from the module's own documents (no RTO-144 sheet yet). Every contact, with where it was read: [`RTO.json`](RTO.json).

| Pin | Signal | Kind | Pair | Confidence |
|---|---|---|---|---|
| 2 |  | unread |  | low |
| 12 | NC | nc |  | high |
| 15 | NC | nc |  | high |
| 16 | NC | nc |  | high |
| 19 | -25V | power |  | high |
| 22 | CHASSIS | ground |  | high |
| 25 | V COM | ground |  | high |

## Manuals and documents

_Manuals and manual pages, price lists, RTO-144 connection sheets, brochures, ads and other document scans._

<table>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKcE9zdTdNQ0JJczg/view?resourcekey=0-jbFWCPT0SSA9ftcvrMIyVQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKcE9zdTdNQ0JJczg&resourcekey=0-jbFWCPT0SSA9ftcvrMIyVQ" width="240" alt="19xx - M522 - 522A - Equalizer (2).pdf"></a><br><sub>19xx - M522 - 522A - Equalizer (2)</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKU2IyR0VBWmxkRkE/view?resourcekey=0-dMHbkNV8zvf3R6VxIVlX5Q" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKU2IyR0VBWmxkRkE&resourcekey=0-dMHbkNV8zvf3R6VxIVlX5Q" width="240" alt="19xx - M522 - 522A - Equalizer.pdf"></a><br><sub>19xx - M522 - 522A - Equalizer</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKck5Db2pfZll2aHc/view?resourcekey=0--AH0g4GSAOhyzluZ8gjVpw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKck5Db2pfZll2aHc&resourcekey=0--AH0g4GSAOhyzluZ8gjVpw" width="240" alt="19xx - M522 - 522A - P001 - Title Page.jpg"></a><br><sub>19xx - M522 - 522A - P001 - Title Page</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKWGl2ZDZ5YnhDT1U/view?resourcekey=0-IUtWD422m3TNDq1yEKqQog" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKWGl2ZDZ5YnhDT1U&resourcekey=0-IUtWD422m3TNDq1yEKqQog" width="240" alt="19xx - M522 - 522A - P002.jpg"></a><br><sub>19xx - M522 - 522A - P002</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKWTFyOE1iYVBuWTg/view?resourcekey=0-hU_KR9ohOI9ZYqa4SiDd_A" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKWTFyOE1iYVBuWTg&resourcekey=0-hU_KR9ohOI9ZYqa4SiDd_A" width="240" alt="19xx - M522 - 522A - P003 - 1-1.jpg"></a><br><sub>19xx - M522 - 522A - P003 - 1-1</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKcmxtRlE4VmliWEE/view?resourcekey=0-rPVVdrNcdS4xuhoL4eUPkg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKcmxtRlE4VmliWEE&resourcekey=0-rPVVdrNcdS4xuhoL4eUPkg" width="240" alt="19xx - M522 - 522A - P004 - 2-1.jpg"></a><br><sub>19xx - M522 - 522A - P004 - 2-1</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKUnVQU0RjSVV5bkU/view?resourcekey=0-TwzaWilXEnnmW9KrkhSHCA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKUnVQU0RjSVV5bkU&resourcekey=0-TwzaWilXEnnmW9KrkhSHCA" width="240" alt="19xx - M522 - 522A - P005 - 3-1.jpg"></a><br><sub>19xx - M522 - 522A - P005 - 3-1</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKS01PVTNRM2xrbmM/view?resourcekey=0-_8KWokLNofWq7a8m76X6LA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKS01PVTNRM2xrbmM&resourcekey=0-_8KWokLNofWq7a8m76X6LA" width="240" alt="19xx - M522 - 522A - P006 - 3-2.jpg"></a><br><sub>19xx - M522 - 522A - P006 - 3-2</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKUjA2TEtUazBpSVU/view?resourcekey=0-UjcpJkMdwprdaqybgewFzQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKUjA2TEtUazBpSVU&resourcekey=0-UjcpJkMdwprdaqybgewFzQ" width="240" alt="19xx - M522 - 522A - P007 - 4-1.jpg"></a><br><sub>19xx - M522 - 522A - P007 - 4-1</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKdVZjRkVLbUVqams/view?resourcekey=0-afRA8BuX_NbL2IaHoLREYA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKdVZjRkVLbUVqams&resourcekey=0-afRA8BuX_NbL2IaHoLREYA" width="240" alt="19xx - M522 - 522A - P008 - 4-2.jpg"></a><br><sub>19xx - M522 - 522A - P008 - 4-2</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKQUxINGc1S2ZPX2c/view?resourcekey=0-VzUySXeXLLXMlbJR2SEb0g" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKQUxINGc1S2ZPX2c&resourcekey=0-VzUySXeXLLXMlbJR2SEb0g" width="240" alt="19xx - M522 - 522A - P009 - 5-1.jpg"></a><br><sub>19xx - M522 - 522A - P009 - 5-1</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKVVJZSF9xc0hIMVU/view?resourcekey=0--hMvx0EqzQQGPLoe70-ZiQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKVVJZSF9xc0hIMVU&resourcekey=0--hMvx0EqzQQGPLoe70-ZiQ" width="240" alt="19xx - M522 - 522A - P010 - 5-2.jpg"></a><br><sub>19xx - M522 - 522A - P010 - 5-2</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKdmtPZGhKUExGMm8/view?resourcekey=0-MzgbaOgVb1ayN3xKr2Pnrg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKdmtPZGhKUExGMm8&resourcekey=0-MzgbaOgVb1ayN3xKr2Pnrg" width="240" alt="19xx - M522 - 522A - P011 - 5-3.jpg"></a><br><sub>19xx - M522 - 522A - P011 - 5-3</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKd1ZocjZZTWNoY2M/view?resourcekey=0-0CrJ51-GFrAYyQyE5Bas8w" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKd1ZocjZZTWNoY2M&resourcekey=0-0CrJ51-GFrAYyQyE5Bas8w" width="240" alt="19xx - M522 - 522A - P012 - 6-1.jpg"></a><br><sub>19xx - M522 - 522A - P012 - 6-1</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKeV9BajhlUHJ2bmM/view?resourcekey=0-D9X7IR6JZp3TVjhiBiHirQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKeV9BajhlUHJ2bmM&resourcekey=0-D9X7IR6JZp3TVjhiBiHirQ" width="240" alt="19xx - M522 - 522A - P013 - 6-2.jpg"></a><br><sub>19xx - M522 - 522A - P013 - 6-2</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKc1hscGE2bmVnMjQ/view?resourcekey=0-JjytWdOCnnK7GC-CHGveNw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKc1hscGE2bmVnMjQ&resourcekey=0-JjytWdOCnnK7GC-CHGveNw" width="240" alt="19xx - M522 - 522A - P014 - 6-3.jpg"></a><br><sub>19xx - M522 - 522A - P014 - 6-3</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKOUM3TFlHTVZQRkU/view?resourcekey=0-_7o2kpVN8QwelnLpH7EqUA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKOUM3TFlHTVZQRkU&resourcekey=0-_7o2kpVN8QwelnLpH7EqUA" width="240" alt="19xx - M522 - 522A - P015 - 6-4.jpg"></a><br><sub>19xx - M522 - 522A - P015 - 6-4</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKZWVIOTFtWUtsWU0/view?resourcekey=0-Vw4y7lRGFHf7lIr4_4Mvxw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKZWVIOTFtWUtsWU0&resourcekey=0-Vw4y7lRGFHf7lIr4_4Mvxw" width="240" alt="19xx - M522 - 522A - P016 - 6-5.jpg"></a><br><sub>19xx - M522 - 522A - P016 - 6-5</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKOHByb3l4V045MDQ/view?resourcekey=0-9e6bv895VW7R9cBqzfgY_g" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKOHByb3l4V045MDQ&resourcekey=0-9e6bv895VW7R9cBqzfgY_g" width="240" alt="19xx - M522 - 522A - P017 - 6-6.jpg"></a><br><sub>19xx - M522 - 522A - P017 - 6-6</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKMGN5eGVSN0xvZzA/view?resourcekey=0-PTukUTOsn_pVcwmsbKy1Kg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKMGN5eGVSN0xvZzA&resourcekey=0-PTukUTOsn_pVcwmsbKy1Kg" width="240" alt="19xx - M522 - 522A - P018 - 6-7.jpg"></a><br><sub>19xx - M522 - 522A - P018 - 6-7</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKeVFEUFExSHFMN1k/view?resourcekey=0-W0ZwRHQKGi7HEC_pTncB0w" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKeVFEUFExSHFMN1k&resourcekey=0-W0ZwRHQKGi7HEC_pTncB0w" width="240" alt="19xx - M522 - 522A - P019 - 6-8.jpg"></a><br><sub>19xx - M522 - 522A - P019 - 6-8</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKOEoxb0lNWjh6MnM/view?resourcekey=0-gemZspARFbeLmvxmc1nDFQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKOEoxb0lNWjh6MnM&resourcekey=0-gemZspARFbeLmvxmc1nDFQ" width="240" alt="19xx - M522 - 522A - P020 - 6-9.jpg"></a><br><sub>19xx - M522 - 522A - P020 - 6-9</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKa1lwR3hhWUM3OUk/view?resourcekey=0-03qtDFMziLO1ynUGqJFw7A" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKa1lwR3hhWUM3OUk&resourcekey=0-03qtDFMziLO1ynUGqJFw7A" width="240" alt="19xx - M522 - 522A - P021 - 6-10.jpg"></a><br><sub>19xx - M522 - 522A - P021 - 6-10</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKamp5ZW5fQmVmZEE/view?resourcekey=0-aPSJj8H2iwP3IT8fuqdoow" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKamp5ZW5fQmVmZEE&resourcekey=0-aPSJj8H2iwP3IT8fuqdoow" width="240" alt="19xx - M522 - 522A - P022 - 7-1.jpg"></a><br><sub>19xx - M522 - 522A - P022 - 7-1</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKZ3l6Z2NXT2ktNUk/view?resourcekey=0-HsHhWpR-zGehbouq6KYoIw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKZ3l6Z2NXT2ktNUk&resourcekey=0-HsHhWpR-zGehbouq6KYoIw" width="240" alt="19xx - M522 - A B - P01.jpg"></a><br><sub>19xx - M522 - A B - P01</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKVzZ1RHlsdXFHdmc/view?resourcekey=0-n_M_wAnYqeNu_ij0fNxHIw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKVzZ1RHlsdXFHdmc&resourcekey=0-n_M_wAnYqeNu_ij0fNxHIw" width="240" alt="19xx - M522 - A B - P02.jpg"></a><br><sub>19xx - M522 - A B - P02</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKdWdQZmxMNi0zMW8/view?resourcekey=0-oJ8bvRII1Qk3CF7Vo5zB_w" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKdWdQZmxMNi0zMW8&resourcekey=0-oJ8bvRII1Qk3CF7Vo5zB_w" width="240" alt="19xx - M522 - A B - P03.jpg"></a><br><sub>19xx - M522 - A B - P03</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKdGlfb3pHUk11Tjg/view?resourcekey=0-uFmcCjH_iYSxbGzoZKP3sg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKdGlfb3pHUk11Tjg&resourcekey=0-uFmcCjH_iYSxbGzoZKP3sg" width="240" alt="19xx - M522 - A B - P04.jpg"></a><br><sub>19xx - M522 - A B - P04</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKRUdyZ3JHTDNNOWM/view?resourcekey=0-0623F8c5gFfkMCI0uKp_Ug" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKRUdyZ3JHTDNNOWM&resourcekey=0-0623F8c5gFfkMCI0uKp_Ug" width="240" alt="19xx - M522 - A B - P05.jpg"></a><br><sub>19xx - M522 - A B - P05</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKdXRkNnBpSXdsRmc/view?resourcekey=0-akrErjdtnf-3gBcMHF4GwA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKdXRkNnBpSXdsRmc&resourcekey=0-akrErjdtnf-3gBcMHF4GwA" width="240" alt="19xx - M522 - A B - P06.jpg"></a><br><sub>19xx - M522 - A B - P06</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKTE1aVUdobGplSk0/view?resourcekey=0-Jh60EOKc0Mg8TMvYUoycew" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKTE1aVUdobGplSk0&resourcekey=0-Jh60EOKc0Mg8TMvYUoycew" width="240" alt="19xx - M522 - A B - P07.jpg"></a><br><sub>19xx - M522 - A B - P07</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKbE5neGQ1aGRsS1k/view?resourcekey=0-8uDu02w3NZUo_InoguEDhw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKbE5neGQ1aGRsS1k&resourcekey=0-8uDu02w3NZUo_InoguEDhw" width="240" alt="19xx - M522 - A B - P08.jpg"></a><br><sub>19xx - M522 - A B - P08</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKalBsRktQZVZmVkU/view?resourcekey=0-na2YKoI6jEVGu5ueq_SJdg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKalBsRktQZVZmVkU&resourcekey=0-na2YKoI6jEVGu5ueq_SJdg" width="240" alt="19xx - M522 - A B - P10.jpg"></a><br><sub>19xx - M522 - A B - P10</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKbHRIZHFndTYzdWs/view?resourcekey=0-CaPLUWsPqbCGbRGBD_iMJg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKbHRIZHFndTYzdWs&resourcekey=0-CaPLUWsPqbCGbRGBD_iMJg" width="240" alt="19xx - M522 - A B - P11.jpg"></a><br><sub>19xx - M522 - A B - P11</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKaHI4UVBiOHZPSE0/view?resourcekey=0-jqEgm25SAL-e00KKJnhzOw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKaHI4UVBiOHZPSE0&resourcekey=0-jqEgm25SAL-e00KKJnhzOw" width="240" alt="19xx - M522 - A B - P12.jpg"></a><br><sub>19xx - M522 - A B - P12</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKMm81V3Q1X1M3NTA/view?resourcekey=0-yyUlbdxUIVYak6bBnbcQ0g" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKMm81V3Q1X1M3NTA&resourcekey=0-yyUlbdxUIVYak6bBnbcQ0g" width="240" alt="19xx - M522 - A B - P13.jpg"></a><br><sub>19xx - M522 - A B - P13</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKZEMyMGNHRXNEcVU/view?resourcekey=0-qBls98D2g049_Sp1Yy6XZQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKZEMyMGNHRXNEcVU&resourcekey=0-qBls98D2g049_Sp1Yy6XZQ" width="240" alt="19xx - M522 - A B - P15.jpg"></a><br><sub>19xx - M522 - A B - P15</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKSFlBUl9ZS09DazQ/view?resourcekey=0-I8FDuiFdKoCCwVjh6dPVEA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKSFlBUl9ZS09DazQ&resourcekey=0-I8FDuiFdKoCCwVjh6dPVEA" width="240" alt="19xx - M522 - A B - P16.jpg"></a><br><sub>19xx - M522 - A B - P16</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKdi1OX1R3LW9rVU0/view?resourcekey=0-VS2ejPVK5V-dK0-e20o6gg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKdi1OX1R3LW9rVU0&resourcekey=0-VS2ejPVK5V-dK0-e20o6gg" width="240" alt="19xx - M522 - A B - P17.jpg"></a><br><sub>19xx - M522 - A B - P17</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKNlFNaF8tRHktYU0/view?resourcekey=0-9KkRmoJAJ54sCczPlgEjng" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKNlFNaF8tRHktYU0&resourcekey=0-9KkRmoJAJ54sCczPlgEjng" width="240" alt="19xx - M522 - A B - P18.jpg"></a><br><sub>19xx - M522 - A B - P18</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKRk9uUUFMSHN6NWs/view?resourcekey=0-lJj9wE69ZJbzM-_k_6va0A" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKRk9uUUFMSHN6NWs&resourcekey=0-lJj9wE69ZJbzM-_k_6va0A" width="240" alt="19xx - M522 - AD - WBSPS - AD - LS series 003.jpg"></a><br><sub>19xx - M522 - AD - WBSPS - AD - LS series 003</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKbFk3ZWlfQTQxdHc/view?resourcekey=0-HhWPKcg7Ls5SELA1psGokQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKbFk3ZWlfQTQxdHc&resourcekey=0-HhWPKcg7Ls5SELA1psGokQ" width="240" alt="19xx - M522 - DOC - 004.jpg"></a><br><sub>19xx - M522 - DOC - 004</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKaVExUlNPcU5VTkk/view?resourcekey=0-99-0K0XkkijrSRAOK8Vz1w" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKaVExUlNPcU5VTkk&resourcekey=0-99-0K0XkkijrSRAOK8Vz1w" width="240" alt="19xx - M522 - DOC - 007.jpg"></a><br><sub>19xx - M522 - DOC - 007</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKT1JzUi1hczZrekU/view?resourcekey=0-c_DWul-nM1uVcirXGJnviQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKT1JzUi1hczZrekU&resourcekey=0-c_DWul-nM1uVcirXGJnviQ" width="240" alt="19xx - M522 - DOC - 011.jpg"></a><br><sub>19xx - M522 - DOC - 011</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKeU5PVEZWZnowbDQ/view?resourcekey=0-ZReLvKRYBLvxwEMXUwSw9w" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKeU5PVEZWZnowbDQ&resourcekey=0-ZReLvKRYBLvxwEMXUwSw9w" width="240" alt="19xx - M522 - DOC - 018.jpg"></a><br><sub>19xx - M522 - DOC - 018</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKcDV5R29Vc0pEQWs/view?resourcekey=0-32OeuYY1JB48dWStBmHEBw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKcDV5R29Vc0pEQWs&resourcekey=0-32OeuYY1JB48dWStBmHEBw" width="240" alt="19xx - M522 - DOC - 023.jpg"></a><br><sub>19xx - M522 - DOC - 023</sub></td></tr>
</table>

Shared privately on Google Drive (opens after sign-in): [1986|19 · DOC - What a manual inside looks like](https://drive.google.com/file/d/0B0yR0b5T78SKYm9Db0hhZjhZbFk/view?resourcekey=0-FydTVX9n2lEDUj4kxe5M3w) · [19xx - M522 - A B - P09](https://drive.google.com/file/d/0B0yR0b5T78SKZjZyQ0FSS0hHV3M/view?resourcekey=0-2j4VdVRCvKjASOeW_3YzLg)

## KiCad

_KiCad: a schematic (`.kicad_sch`) traced from each electrical drawing, the module symbol (`.kicad_sym`) and its PCB projects. Traced schematics are the line work only: redraw with symbols over them._

- [19xx - 522-01-001 - EQUALIZER MODULE FUNCTIONAL - ISS 1.kicad_sch](KICAD/19xx%20-%20522-01-001%20-%20EQUALIZER%20MODULE%20FUNCTIONAL%20-%20ISS%201.kicad_sch)
- [19xx - 522-01-002 - EQUALIZER MODULE FUNCTIONAL - ISS 1.kicad_sch](KICAD/19xx%20-%20522-01-002%20-%20EQUALIZER%20MODULE%20FUNCTIONAL%20-%20ISS%201.kicad_sch)
- [19xx - 522-02-001 - EQUALIZER MODULE SCHEMATIC - ISS 3.kicad_sch](KICAD/19xx%20-%20522-02-001%20-%20EQUALIZER%20MODULE%20SCHEMATIC%20-%20ISS%203.kicad_sch)
- [19xx - 522-02-002 - EQUALIZER MODULE SCHEMATIC - ISS 3.kicad_sch](KICAD/19xx%20-%20522-02-002%20-%20EQUALIZER%20MODULE%20SCHEMATIC%20-%20ISS%203.kicad_sch)
- [19xx - 522-02-003 - MONO EQUALIZER MODULE SCHEMATIC - ISS 1.kicad_sch](KICAD/19xx%20-%20522-02-003%20-%20MONO%20EQUALIZER%20MODULE%20SCHEMATIC%20-%20ISS%201.kicad_sch)
- [19xx - M522 - 522-01-001 - EQUALIZER MODULE FUNCTIONAL.kicad_sch](KICAD/19xx%20-%20M522%20-%20522-01-001%20-%20EQUALIZER%20MODULE%20FUNCTIONAL.kicad_sch)
- [19xx - M522 - 522-01-001.kicad_sch](KICAD/19xx%20-%20M522%20-%20522-01-001.kicad_sch)
- [19xx - M522 - 522-01-002 - EQUALIZER MODULE FUNC TIONAL.kicad_sch](KICAD/19xx%20-%20M522%20-%20522-01-002%20-%20EQUALIZER%20MODULE%20FUNC%20TIONAL.kicad_sch)
- [19xx - M522 - 522-01-002.kicad_sch](KICAD/19xx%20-%20M522%20-%20522-01-002.kicad_sch)
- [19xx - M522 - 522-02-001 - UNLESS OTHERWISE SPECIFIED COM LAST COMPONENT DESIGNAT IONS.kicad_sch](KICAD/19xx%20-%20M522%20-%20522-02-001%20-%20UNLESS%20OTHERWISE%20SPECIFIED%20COM%20LAST%20COMPONENT%20DESIGNAT%20IONS.kicad_sch)
- [19xx - M522 - 522-02-001 - WUKS ALL CAPACITORS ARE.kicad_sch](KICAD/19xx%20-%20M522%20-%20522-02-001%20-%20WUKS%20ALL%20CAPACITORS%20ARE.kicad_sch)
- [19xx - M522 - 522-02-002 - ALL CAPACITORS ARE UNLESS OTHERWISE SPEC.kicad_sch](KICAD/19xx%20-%20M522%20-%20522-02-002%20-%20ALL%20CAPACITORS%20ARE%20UNLESS%20OTHERWISE%20SPEC.kicad_sch)
- [19xx - M522 - 522-02-002 - UNLESS OTHERWISE SPEC IFIED LAST COMPONENT DESIGNATIONS.kicad_sch](KICAD/19xx%20-%20M522%20-%20522-02-002%20-%20UNLESS%20OTHERWISE%20SPEC%20IFIED%20LAST%20COMPONENT%20DESIGNATIONS.kicad_sch)
- [19xx - M522 - 522A - Equalizer (2) p26.kicad_sch](KICAD/19xx%20-%20M522%20-%20522A%20-%20Equalizer%20(2)%20p26.kicad_sch)
- [19xx - M522 - 522A - Equalizer (2) p30.kicad_sch](KICAD/19xx%20-%20M522%20-%20522A%20-%20Equalizer%20(2)%20p30.kicad_sch)
- [19xx - M522 - 522A - Equalizer (2) p32.kicad_sch](KICAD/19xx%20-%20M522%20-%20522A%20-%20Equalizer%20(2)%20p32.kicad_sch)
- [19xx - M522 - 522A - Equalizer p28.kicad_sch](KICAD/19xx%20-%20M522%20-%20522A%20-%20Equalizer%20p28.kicad_sch)
- [19xx - M522 - 522A - Equalizer p32.kicad_sch](KICAD/19xx%20-%20M522%20-%20522A%20-%20Equalizer%20p32.kicad_sch)
- [19xx - M522 - A B - P19 - Filter Schematic.kicad_sch](KICAD/19xx%20-%20M522%20-%20A%20B%20-%20P19%20-%20Filter%20Schematic.kicad_sch)
- [19xx - M522 - A B - P20 - EQ Schematic.kicad_sch](KICAD/19xx%20-%20M522%20-%20A%20B%20-%20P20%20-%20EQ%20Schematic.kicad_sch)
- [M522.kicad_sym](KICAD/M522.kicad_sym)
- [index.html](KICAD/index.html)

## Software

- [index.html](SOFTWARE/index.html)

---
Archive: Anthony Peter Kuzub · [WBSps.ca](https://WBSps.ca) · [WBSps.Kuzub.com](https://WBSps.Kuzub.com)
