 # Bit Bounties - Verbetervoorstellen


## Verbetervoorstel 1: Testen
Bij de verbeterpunten van opdracht 4 hebben we drie belangrijke verbetervoorstellen geïdentificeerd. Hieronder wordt uitgelegd waarom deze verbeteringen nodig zijn en hoe ze geïmplementeerd kunnen worden.
### Waarom moet dit verbeterd worden?

### 1.1 **AuthAdmin probleem**:
   - **Probleem**: Uit de AuthAdminTest test bleek dat de Studentent bij de bedrijfspagina's konden komen.
   - **Impact**: Studenten die toegang hebben tot de bedrijfspagina's kunnen gegevens zien die ze normaal gesproken niet mogen inzien, wat betekent dat de gegevens van de bedrijven niet veilig zijn.

### 1.2 **Responsive gedrag onder verschillende apparaten**:
   - **Probleem**: Het platform biedt geen consistente gebruikerservaring op verschillende apparaten en schermformaten.
   - **Impact**: Gebruikers ervaren frustratie en mogelijk gebruiksonderbrekingen, wat de algehele tevredenheid beïnvloedt.

### 1.3 **Vereenvoudiging van het Registratieproces**:
   - **Probleem**: Het huidige authenticatieproces is te complex en veroorzaakt verwarring bij nieuwe gebruikers.
   - **Impact**: Potentiële gebruikers kunnen afzien van registratie, wat de groei van het platform beperkt.

### Voorgestelde Verbeterstappen:

### Voor AuthAdmin probleem

**Optimalisatie van de AuthAdmin**:
   - Voeg een verificatiemechanisme toe waarbij alleen studenten met een geldig Student_ID en bedrijven met een Bedrijf_ID toegang krijgen tot hun respectieve gegevens.
   - Deze ID's moeten ook worden gebruikt om de juiste rollen en rechten toe te passen.

#### Wat moeten we doen om dit te kunnen oplossen/implementeren:
   - Database tabelen updaten door een Studen_ID kolom en een Bedrijf_id kolum toe te voegen.
   - Backend autorisatie aanpassen door de gebruiker te controleren in de middleware of de gebruiker de juiste rol heeft.

### Voor Responsive gedrag onder verschillende apparaten

**Verbeteringen aanpassen aan verschillende schermgroottes**:
   - Ontwikkel en implementeer een responsive design dat zich automatisch aanpast aan verschillende apparaten.

#### Wat moeten we doen om dit te kunnen oplossen/implementeren:
   - Gebruik media queries om responsieve stijlen te creëren voor verschillende schermformaten.
   - Voer grondige tests uit met tools zoals BrowserStack om compatibiliteit en responsiviteit te garanderen.

### Voor Vereenvoudiging van het Registratieproces

**Vereenvoudiging van het Registratieproces**:
   - Verminder het aantal vereiste stappen om een account aan te maken.
   - Introduceer social login mogelijkheden om het makkelijker te maken voor gebruikers om zich te registreren met bestaande accounts zoals GitHub.

#### Wat moeten we doen om dit te kunnen oplossen/implementeren:
   - Analyseer het huidige registratieproces om onnodige stappen te identificeren en elimineren.
   - Integreer OAuth voor social logins, beginnend met Github.

## Verbetervoorstel 2: Oplevering

Bij de Demo`s hadden we steeds de zelfde feedback.

### 2.1 **Flow van het platform**:

### Waarom moet dit verbeterd worden?
- **Probleem**: Tijdens demos bleek dat de flow van het platform niet duidelijk werd getoond aan de gebruiker, wat leidde tot verwarring.
- **Impact**: Onvoldoende demonstratie van de platformfunctionaliteit kan de acceptatie en begrip van het platform door potentiële gebruikers verminderen.

**Voorgestelde Verbeterstappen:**
 - Maak een gestructureerde guide pagina die uitlegt hoe het plaftorm in elkaar zit en hoe het platform werkt. De pagina moet vooral de belangerijkste functies benadruken.

### 2.2 **README voor Repository**:

### Waarom moet dit verbeterd worden?
- **Probleem**: Na het maken van een test kreeg de gebruiker wel een repository, maar ontbrak een duidelijke beschrijving in de README, wat het begrip van de test inhoud belemmerde.
- **Impact**: Gebrek aan documentatie kan leiden tot verwarring en verminderde efficiëntie bij het gebruik van de testrepositories.

**Voorgestelde Verbeterstappen:**
- Automatiseer het proces om een README te genereren en deze toe te voegen aan elke nieuw gecreëerde testrepository.

### 2.3 **Ontbrekende API-routes voor de Front-End**:

### Waarom moet dit verbeterd worden?
- **Probleem**: Tijdens de oplevering werd ontdekt dat bepaalde API-routes ontbraken, waardoor functionaliteiten niet volledig beschikbaar waren voor de front-end.
- **Impact**: Ontbrekende API-routes kunnen de bruikbaarheid van het platform beperken en de gebruikerservaring negatief beïnvloeden.

**Voorgestelde Verbeterstappen:**
- Identificeer de ontbrekende API-routes en implementeer ze om volledige functionaliteit voor de front-end te garanderen.
## Verbetervoorstel 3: Reflectie

### 3.1 **Verbetering van Communicatie**:

### Waarom moet dit verbeterd worden?
- **Probleem**: De communicatie tijdens het ontwikkelingsproces was niet optimaal, wat leidde tot misverstanden en vertragingen.
- **Impact**: Gebrekkige communicatie kan de samenwerking belemmeren en de efficiëntie van het ontwikkelingsteam verminderen.

**Voorgestelde Verbeterstappen:**
   - Meer Daily Standups doen waar je uitlegt waar je mee bezig bent of waar je mee vast zit.
   - Gebruik tools zoals Mattermost of Whatsapp voor communicatie en maak duidelijke afspraken over het gebruik ervan.


### 3.2 **Versnelling van Werktempo**:

### Waarom moet dit verbeterd worden?
- **Probleem**: Het werktempo was te langzaam tijdens het ontwikkelingsproces, waardoor deadlines niet werden gehaald.
- **Impact**: Trage vooruitgang kan de algehele productiviteit van het team verminderen en de tijdlijn voor projectoplevering verlengen.

**Voorgestelde Verbeterstappen:**
   - Maak haalbare deadlines en bespreek het met de Project Manager als je een deadline niet gaat halen.
   - Houd de voortgang regelmatig in de gaten en stuur bij waar nodig om te voorkomen dat het werktempo vertraagt.


### 3.3 **Verheldering van Rollen in Meetings**:

### Waarom moet dit verbeterd worden?
- **Probleem**: Rollen in meetings waren heel onduidelijk, wat leidde tot verwarring en inefficiënte vergaderingen.
- **Impact**: Onduidelijke rollen kunnen leiden tot een gebrek aan focus, vertragingen in besluitvorming en verminderde betrokkenheid van teamleden.

**Voorgestelde Verbeterstappen:**
- **Roldefinitie vóór elke vergadering**:
   - Wijs duidelijk rollen toe aan elk teamlid voordat de vergadering begint, zoals notulist, facilitator, tijdwaarnemer, etc.
- **Vastleggen van verantwoordelijkheden**:
   - Definieer de verantwoordelijkheden van elke rol en communiceer deze aan alle deelnemers om verwarring te voorkomen.
- **Actieve deelname aan rollen**:
   - Moedig teamleden aan om actief deel te nemen aan hun toegewezen rollen en verantwoordelijkheden tijdens de vergadering.
- **Evalueren en aanpassen**:
   - Evalueer regelmatig de effectiviteit van de rollen en pas ze aan indien nodig op basis van feedback van het team.

## Conclusie
Door deze verbetervoorstellen te implementeren, kunnen we de responsiviteit, gebruiksvriendelijkheid en efficiëntie van het platform verbeteren. Het is essentieel om deze voorstellen te blijven evalueren en aan te passen op basis van gebruikersfeedback en verdere reflecties of demo`s om een continue verbetering van het product te behouden.


