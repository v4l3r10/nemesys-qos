NeMeSys Client
==============
The Speed Analisys tool for Italian connections  [site](https://www.misurainternet.it/nemesys.php).


Installation instructions
=========================

Quelle che seguono sono le intruzioni di installazione di NeMeSys su varie piattaforme. NeMeSys è sviluppato in Python e per funzionare ha bisogno delle librerie standard di Python_ 2.6 (2.6.4 e successive) e della libreria aggiuntiva M2Crypto.

Windows
-------

Se si dispone dei sorgenti di NeMeSys, per eseguire NeMeSys occorre installare preventivamente Python 2.6. L'installazione più semplice prevede l'uso dei binari pre-compilati ufficiali reperibili alla pagina: http://www.python.org/download/

E' utile inserire l'eseguibile di Python nel PATH del sistema. Inseriamo per questo la cartella di installazione di Python (generalmente ``C:\Python26``) nel PATH.

Prima di usare NeMeSys occorre installare del software necessario per la firma delle misure.

Tuttavia, se non si desidera inviare misure al repository, si può omettere l'installazione del software aggiuntivo, ma si deve avere l'accortezza di eseguire ''executer.py'' con l'opzione che disabilita l'invio delle misure.

Se invece desideriamo inviare misure al repository server, occorre installare OpenSSL_ e M2Crypto_.

OpenSSL
```````

Per installare OpenSSL_ (versione 0.98 o successive) possiamo scaricare ed installare i binari pre-compilati da http://www.slproweb.com/products/Win32OpenSSL.html prendiamo il pacchetto *Win32 OpenSSL v0.9.8m Light*

Probabilmente avremo bisogno di installare preventivamente il pacchetto *Visual C++ 2008 Redistributables*.


M2Crypto
````````
Dovo aver installato OpenSSL, possiamo procedere con l'installazione di M2Crypto_.

Scarichiamo e installiamo i binari precompilati prendendoli da http://chandlerproject.org/Projects/MeTooCrypto#Downloads

Linux
-----

Le distribuzioni Linux più diffuse hanno già installate di default le librerie standard di Python. Per inviare le misure firmate, tuttavia, abbiamo bisogno di installare M2Crypto_.

In distribuzioni Debian-like possiamo installare Python e M2Crypto usando il comando::

  sudo apt-get install python python-m2crypto

Una volta installati i pacchetti necessari, verifichiamo che tutto sia installato correttamente e che la versione di Python sia corretta::

  $ python
  Python 2.6.4 (r264:75706, Dec  7 2009, 18:45:15) 
  [GCC 4.4.1] on linux2
  Type "help", "copyright", "credits" or "license" for more information.
  >>> import M2Crypto
  >>>

Versioni di Python 2.6 uguali o successive alla 4 sono compatibili con NeMeSys. Il test di importazione delle librerie M2Crypto non deve dare eccezioni.

.. _Python: http://www.python.org/
.. _M2Crypto: http://chandlerproject.org/Projects/MeTooCrypto
.. _OpenSSL: http://www.openssl.org/



