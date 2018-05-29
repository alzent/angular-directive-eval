Starten:
--
ng serve
... und im Browser aubrufen


Dieses Eal-Projekt verdeutlicht das Konzept der Directiven.
---


Directive erstellen
----
ng new angular-directive-eval
cd angular-directive-eval
ng generate directive sizer // wobei 'sizer' der Name der Directive ist!


Funktionsweise
---
* Über app.module.ts wird 'SizerDirective' eingebunden.

* Diese Directive ist in sizer.directive.ts definiert
    * der Selector zur Identifizierung der Direktive lautet: 'sizer'
    * wird der Selector aufgerufen, so erfolgt ein Call der LifyCycle-Funktion 'ngOnInit'. Hier ist die Funktionalität der Directive definiert.

* Um eine Directive zu verwenden wird diese als Attribute eines DOM-Elements angegeben:
    * Siehe app.component.html => 
        * <div sizer="72px">







