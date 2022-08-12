# wtg_storage

## Kern-Anforderungen
<ol>
  <li> Neue Kostüme anlegen, mit Beschreibung, Stückzahl und Bild </li>
  <li> Kostüm soll von einem Mitglied ausgeliehen werden können ausleihen </li> 
  <li> Liste aller Kostüme anzeigen lassen </li>
  <li> Detailansicht pro Kostüm mit momentan vorhandener Stückzahl und wer was ausgeliehen hat </li>
  <li> Liste aller ausgeliehenen Kostüme anzeigen lassen </li>
  <li> Liste aller Mitglieder anzeigen lassen mit Anzeige ob noch Kostüme ausgeliehen sind </li>
  <li> Liste aller Mitglieder anzeigen lassen, die momentan etwas ausgeliehen haben </li>
  <li> Kostüme/Mitglieder suchen </li>
  <li> Kostüme/Mitglieder sollen geändert werden können (z.B. Austritt eines Mitglieds, Verlust/Defekt eines Kostüms </li>
</ol>
<br>

## Mögliche Erweiterungen 
<ul>
  <li> Ablageort von Kostümen speichern (also welcher Schrank) </li>
  <li> Räumchen visualisieren, sodass Ablageort eines Kostüms auf Karte markiert ist </li>
</ul>
<br>

## Datenbank
items:<br>
<ul>
	<li>id PRIMARY KEY</li>
	<li>description</li>
	<li>numberOfPieces</li>
	<li>imageID</li>
	<li>createdTime</li>
</ul>
<br>

members: <br>
<ul>
	<li>id PRIMARY KEY</li>
	<li>name</li>
	<li>givenName</li>
	<li>createdTime</li>
</ul>	
<br>

burrow:<br>
<ul>
	<li>id PRIMARY KEY</li>
	<li>memberID FOREIGN KEY</li>
	<li>itemID FOREIGN KEY</li>
	<li>burrowTime</li>
</ul>
	
