teryt-down
==========

Incorporates https://github.com/fsi-open/teryt-database-bundle
to download TERYT db.

Running
=======

First obatain username / pass creds:

Aby móc korzystać z usługi, należy wysłać email na adres teryt_ws1@stat.gov.pl podając następujące dane:

	Nazwa użytkownika
	Numer telefonu
	Adres email
	Podmiot komercyjny / Administracja publiczna/ Osoba prywatna

Informacja zwrotna do użytkownika zostanie przesłana zaraz po założeniu konta. Dla
środowiska produkcyjnego adresy są następujące:
 Adres usługi produkcyjnej: https://uslugaterytws1.stat.gov.pl/terytws1.svc
 Adres dokumentu wsdl: https://uslugaterytws1.stat.gov.pl/wsdl/terytws1.wsdl

Obtained creds paste here:

fsi_teryt_db:
    api:
        url: "https://uslugaterytws1.stat.gov.pl/wsdl/terytws1.wsdl"
        username: "<your username>"
        password: "<your password>"

Then follow the https://github.com/fsi-open/teryt-database-bundle README like so:

$ cd project
$ php app/console teryt:download:territorial-division
$ php app/console teryt:download:places-dictionary
$ php app/console teryt:download:places
$ php app/console teryt:download:streets


What is it?
===========

A Symfony project created on November 5, 2018, 1:46 am.
