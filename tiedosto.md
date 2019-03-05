SSH komennolla käynnistetään SSH client ohjelma jonka avulla voidaan muodostaa suojattu yhteys SSH serveriin etäkoneella.
SSH käskyä käytetään kun logataan sisään etäkoneeseen, siirretään tiedostoja ja ajetaan komentoja.
SSH-keygen, komennolla luodaan avainpari julkista tunnistautumista varten
SSH:lla kirjauduttaessa voidaan käyttää kohteena user@hostname tai sitten muotoa URI of the form ssh://[user@]hostname[:port]

Esimerkki käskyjen ajamisesta etäkoneella yhdistämisen jälkeen.

Executing remote commands on the server

The ssh command is often also used to remotely execute commands on the remote machine without logging in to a shell prompt. The syntax for this is:

ssh hostname command

For example, to execute the command:

ls /tmp/doc 

on host sample.ssh.com, type the following command at a shell prompt:

ssh sample.ssh.com  ls /tmp/doc

