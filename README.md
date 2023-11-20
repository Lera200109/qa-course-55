Feature: Utilizatorul se poate inregistra cu succes
Scenario1:Utilizatorul poate completa toate campurile cu date personale
GIVEN: Utilizatorul se afla pe pagina inregistraii "Join Today"
WHEN: Utilizatorul completeaza toate campurile libere cu date personale
AND: Utilizatorul merge la urmatorul pas prin click "Next: Location"
AND: Utilizatorul completeaza campurile si merge la urmatorul pas prin click "Next: Devices"
AND: Utilizatorul completeaza campurile si merge la urmatorul pas prin click "Next: Last Step"
AND: Utilizatorul isi creaza o parola si merge la urmatorul pas prin click "Complete Setup"
AND: Utilizatorul selecteaza imagiea solicitata pentru verificare
THEN: Utilizatorul se poate inregistra cu succes



Feature: Utilizatorul nu se poate inregistra cu succes
Scenario1: Utilizatorul nu poate seta o parola standarta
GIVEN: Utilizatorul se afla pe pagina la "Step 4: The last step"
WHEN: Utilizatorul tapeaza o parola alcatuita doar din litere minuscule
THEN: Utilizatorul nu se poate inregistra

Scenario2: Utilizatorul nu se poate inregistra cu succes la validarea afirmatiei ca nu este robot
GIVEN:Utilizatorul se afla pe pagina de validarea afirmatiei ca utilizatorul nu este robot
WHEN: Utilizatorul selecteaza imagini gresite decat cele solicitate
THEN: Utilizatorul nu se poate inregistra.


Feature: Utilizatorul se poate loga cu succes
Scenario1: Utilizatorul se poate loga
GIVEN: Utilizatorul se afla pe pagina de logare
WHEN: Utiliztorul tapeaza loginul si parola
THEN: Utiliazatorul se poate loga cu succes


Feature: Utilizatorul nu se poate loga cu succes
Scenario1: Utilizatorul nu se poate loga cu parola tapata gresit
GIVEN: Utilizatorul se afla pe pagina de logare
WHEN: Utiliztorul tapeaza parola doar cu minuscule
THEN: Utiliazatorul nu se poate loga cu succes

Scenario2: Utilizatorul nu se poate loga cu posta electronica tapata gresit
GIVEN: Utilizatorul se afla pe pagina de logare
WHEN: Utiliztorul tapeaza posta electorinica gresit
THEN: Utiliazatorul nu se poate loga cu succes


Feature: Utilizatorul poate edita informatiile generale al profilului sau
Scenatio 1: Utilizatorul poate edita informatia la diviziunea "PERSONAL"
GIVEN: Utilizatorul se afla pe pagina "PERSONAL:
WHEN: Utilizatorul tapeaza si selecteaza toata informatia persoanala
Then : Utilizatorul editeaza si salveaza cu succes informatia la profil

Scenario2:Utilizatorul poate edita informatia la diviziunea "DEVICES"
GIVEN: Utilizatorul se afla pe pagina "DEVICES"
WHEN: Utilizatorul tapeaza si selecteaza toata informatia persoanala
Then : Utilizatorul editeaza si salveaza cu succes informatia la profil

Scenario3:Utilizatorul poate edita informatia la diviziunea "PAYMENT TESTING"
GIVEN: Utilizatorul se afla pe pagia "PAYMENT TESTING"
WHEN: Utilizatorul tapeaza si selecteaza toata informatia persoanala
Then : Utilizatorul editeaza si salveaza cu succes informatia la profil



Feature: Utilizatorul poate posta un status
Scenario1: Utilizatorul poate tapa un status in forumul "Community"
GIVEN: Utilizatorul se afla pe pagina
WHEN: Utilizatorul tapeaza un text
AND: Utilizatorul da clisk pe butonul "Share status"
THEN: Utilizatorul poate posta un status
