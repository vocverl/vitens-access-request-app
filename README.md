# Vitens Access Request Application

Een single-page web applicatie voor het aanvragen van toegang tot SAP GRC systemen met bijbehorende GRC tools.

## Overzicht

Deze applicatie helpt gebruikers om toegangsverzoeken in te dienen voor SAP GRC systemen binnen Vitens. Het is gebouwd als een demo/prototype om de toegevoegde waarde te laten zien van geautomatiseerde access request workflows.

## Componenten

### Access Request App
- **index.html** - Hoofdapplicatie voor access requests
  - Gebruiksvriendelijke interface
  - Formulier voor toegangsaanvragen
  - Validatie en preview functionaliteit

### GRC Tools

**test-grc-connection.html**
- Test connectiviteit met SAP GRC systemen
- Valideer configuratie
- Debug connection issues

**grc-config.js**
- Configuratie voor GRC connecties
- System endpoints
- Authentication settings

**inspect-excel.html**
- Upload en inspecteer Excel bestanden
- Data preview functionaliteit
- Gebruikt voor GRC data imports

**inspect_bor.py**
- Python script voor BOR (Bill of Rights) analyse
- Parse en valideer BOR bestanden
- Command-line tool

## Gebruik

### Access Request App

1. Open `index.html` in een browser
2. Vul het formulier in met je toegangsverzoek
3. Review en submit

### GRC Connection Tester

1. Open `test-grc-connection.html`
2. Configureer connection settings
3. Test de verbinding

### Excel Inspector

1. Open `inspect-excel.html`
2. Upload een Excel bestand
3. Bekijk de data en structuur

### BOR Inspector

```bash
python inspect_bor.py <bor-file>
```

## Features

- Single-page applicatie (geen server nodig)
- Responsive design
- Client-side validatie
- GRC integratie ready
- Debug en testing tools

## Tech Stack

- HTML5
- JavaScript (vanilla)
- CSS3
- Python (voor BOR inspector)

## Development

Alle tools zijn standalone en vereisen geen build process:
- Open HTML bestanden direct in browser
- Geen dependencies of npm packages nodig
- Python script werkt standalone

## Toekomstige Uitbreidingen

- [ ] Live SAP GRC integratie
- [ ] User authentication
- [ ] Request tracking dashboard
- [ ] Email notifications
- [ ] Approval workflow
- [ ] Integration met HR systemen

## Licentie

Proprietary - Vitens N.V.
