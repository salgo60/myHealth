# myHealth
Fundera över hur olika delar kan kopplas ihop

![AIGubbens Hälsa](image/AIGubbens%20H%C3%A4lsa.jpeg)

1. Apple health
  * dit skriver Withings, Runkeeper 
2. Withings
   * kopplar ihop [WiFi-våg](https://www.clasohlson.com/se/Withings-Body-Smart-badrumsvag-med-kroppsanalys,-WiFi/p/44-5361-2)  och [BPM Vision](https://www.withings.com/en-us/products/bpm-vision) -
   * Skriver till Apple health men inte kommentarer på olika mätningar
   * data med kommentarer kan hämtas från Withings via download email [Withings App - Online Dashboard - Exporting my data](https://support.withings.com/hc/en-us/articles/201491377-Withings-App-Online-Dashboard-Exporting-my-data)
     * betyder att jag kan spåra mätning blodtryck innan medicin, efter medicin, kväll och höger/vänster arm som skrivs som kommentar som ChatGPT tolkar 
3. Foodvisor - hanterar målrider
   - [Foodvisor Exporter](https://github.com/thm01/foodvisor-exporter) - är ett inofficiellt Pythonverktyg som exporterar din Foodvisor-dagbok till Excel, CSV och JSON.
      - Hämtar måltider, livsmedel, mängder, näringsvärden, vatten och tillgängliga aktiviteter för en vald period.
      - Körs lokalt med ett gränssnitt i webbläsaren
      - Kan ge myHealth detaljerad måltidsdata för egen analys
   - * **Foodvisor – registrerar måltider och beräknar näringsintag**
   - **Läser från Apple Hälsa:** träningspass, aktiv energi, träningsminuter och steg.
   - **Skriver till Apple Hälsa:** kontrollera vilka näringsvärden som delas under Foodvisors behörigheter i Hälsa.
4. iWatch mäter puls, sömn, steg, 
   - **Hjärta:** puls, vilopuls och pulsvariabilitet (HRV).
   - **Aktivitet:** steg, gång- och löpdistans, ståtid och uppskattad energiförbrukning.
   - **Träning:** träningspass, tid, distans, tempo, puls och GPS-rutt vid exempelvis löpning och vandring.
   - **Kondition:** uppskattar VO₂ max vid vissa promenader, löp- och vandringspass utomhus.
   - **Sömn:** uppskattar sömntid, vakenperioder och sömnstadier samt registrerar puls och andningsfrekvens under natten.
   - **Beroende på modell och inställningar:** även EKG, syremättnad, handledstemperatur och notiser om tecken på sömnapné.
   - **Apple Hälsa:** sparar mätningarna där, så att de kan kombineras med vikt och blodtryck från Withings och måltidsdata från andra appar som stöder integrationen.
   - **Idé för myHealth:** följa hur mat, motion och sömn hänger ihop med vikt, blodtryck och kondition över tid.
5. [Snore Lab](https://www.snorelab.com/) - snarkning, andning
   * Apple Hälsa
      * läser sömnstadier från Apple Hälsa/Apple Watch
      * skriver Sömn
6. [Mathem](https://www.mathem.se) ?
   * skulle vilja kunna jmf vad som köpts med vad som finns kvar i kylskåpet
   *  * **[HelloFresh](https://www.hellofresh.se) – måltider och recept**
   * skriver till **Apple Hälsa:** 
       * Dietär energi (kalorier)
       * Kolesterol
       * Socker
       * Fiber
       * Kolhydrater
       * Mättat fett
       * Natrium
       * Protein
       * Totalt fett
  * **Läser från Apple Hälsa:** ingen läsbehörighet visas i skärmbilden.
  * **Att kontrollera:** Läsewr Foodvisor detta data?
7. [HelloFresh](https://www.hellofresh.com)
   - Skulle vilja kunna s kalori och näring på levererade maträtter
