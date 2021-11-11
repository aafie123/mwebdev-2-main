# mwebdev-2
Deze repo hoort bij de lessen modern webdevelopment van de gmi-designschool te Amsterdam

 + + + npm gulp test site + + + 
 
Gulp 4 geeft een error in een simpele custom functie, omdat in gulp 4 taken asynchroon uitgevoerd worden.
Dit kan opgelost worden door een callback functie toe te voegen, bijvoorbeeld:
// + + + + + TEST versie 4

function hallo(cb) {

    return console.log('Test gulp versie 4.');
    
    cb();
    
}

exports.hallo = hallo;

Start nu de task met het terminal commando: gulp
