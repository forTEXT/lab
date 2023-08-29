How to change content

Ordner mit Bildern:
- static/images/
	- lab_team : Fotos der Teammitgliedern
	- overview : Sammlung von Labübersichtsversionen auf der Landing Page
	
Ordner zum Ändern von Inhalten je nach Sprache aufgeteilt (de/en)
- content/de/lab_team : infos der Teammitglieder; für jedes Teammitglied ein Ordner mit Markdownfile "bio.md"
			- Bild muss unter gleichem Namen wie Ordnername des Mitglieds unter static/images/lab_team/....png gespeichert werden
			- _index.md enthält die Liste von Studentischen Hilfskräften etc 
- content/de/projekte ;
			- dis_pub_reihen : enthält Publiaktions und D.-Reihen
				- für fortext portal und JCLS wird ein Shortcode auifgerufen (layout/shortcodes/projekt_info)
			- Forschungsprojekte: Forrschungsprojekte
			- Software: CATMA wird über shortcode aufgerufen ("projekt_info.html"
			- Bilder der Projekte liegen unter static/images
			
