# hermes-backup

Krypterade nattdumpar (arenden, redovisning, hermes-zip, redovisning-data med kvittobilagor),
sju rullande platser (dag1..dag7).

Dekryptering:
    gpg --batch --passphrase-file backup-nyckel -d dumpar-dagN.tar.gpg > paket.tar

En fil över 90 MB ligger delad (GitHub tar inte filer över 100 MB). Sätt ihop först:
    cat dumpar-dagN.tar.gpg.del-* > dumpar-dagN.tar.gpg

Nyckeln ligger ALDRIG här.
