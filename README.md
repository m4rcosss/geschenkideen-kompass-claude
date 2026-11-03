# Geschenkideen-Kompass für Claude

![Geschenkideen-Kompass](assets/icon.png)

Dieses Plugin verbindet Claude mit dem [Geschenkideen-Kompass](https://geschenkideen-kompass.de), einem redaktionell gepflegten Katalog mit Hunderten Geschenkideen für Deutschland. Frag nach einem Geschenk für eine Person, ein Alter, einen Anlass oder ein Budget – zum Beispiel „ein Geschenk für eine 6-Jährige unter 20 Euro“ oder „etwas für meinen Papa, der gern grillt“ – und Claude schlägt passende Ideen mit kurzer Begründung, Preisklasse und Link zur Produktseite vor.

## Was das Plugin enthält

- **MCP-Server** `https://geschenkideen-kompass.de/mcp` (Streamable HTTP, ohne Anmeldung). Werkzeuge, alle nur lesend: `find_gifts` (Filter nach Zielgruppe, Kategorie, Interessen, Marke, Alter, Preisklasse, nachhaltig, Suchbegriff), `get_gift` (Details), `similar_gifts` (Alternativen), `search` und `fetch` (Volltextsuche), `list_options` (gültige Filterwerte).
- **Skill** `geschenkberatung`: führt Claude durch eine kurze Geschenkberatung mit diesen Werkzeugen.

## Welche Daten fließen

Das Plugin sendet nur die Suchparameter einer Anfrage (etwa Zielgruppe, Alter, Preisklasse oder Suchbegriff) an den MCP-Server des Geschenkideen-Kompass und bekommt öffentlich sichtbare Inhalte des Katalogs zurück. Es führt keinen Code auf deinem Rechner aus, liest keine lokalen Dateien und nutzt keine Zugangsdaten. Der Server speichert nur, wie oft welches Werkzeug pro Tag aufgerufen wurde – keine Anfragetexte, keine IP-Adressen ([Datenschutz](https://geschenkideen-kompass.de/datenschutz), [Nutzungsbedingungen](https://geschenkideen-kompass.de/nutzungsbedingungen)).

Preise erscheinen nur als Preisklasse oder – wenn tagesaktuell verfügbar – mit Stand. Links führen zur Produktseite auf geschenkideen-kompass.de; Kauf-Links dort sind gekennzeichnete Amazon-Partnerlinks. Gekauft wird nicht über das Plugin.

## Kontakt

Marco Scheel · info@geschenkideen-kompass.de · [Impressum](https://geschenkideen-kompass.de/impressum)
