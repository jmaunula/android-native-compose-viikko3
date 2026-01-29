## MVVM
MVVM jakaa sovelluksen kolmeen osaan: Model (data, esim. Task), View (UI/Composablet) ja ViewModel (logiikka ja UI:n tila).
MVVM tarkoittaa sitä, että UI ei tee itse mitään logiikkaa, vaan se vain näyttää tietoa ja lähettää napin painallukset ViewModelille. ViewModel pitää sovelluksen tilan ja muokkaa dataa, ja kun tila muuttuu, Compose päivittää näkymän automaattisesti. 
Tämä tekee koodista selkeämmän, helpommin testattavan ja helpommin ylläpidettävän.
## StateFlow
StateFlow toimii niin, että se pitää aina viimeisimmän tilan muistissa ja “ilmoittaa” UI:lle kun arvo muuttuu. Compose kuuntelee sitä collectAsState()-toiminnolla ja piirtää ruudun uudestaan, kun data päivittyy.
