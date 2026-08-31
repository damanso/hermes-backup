# hermes-backup

Krypterade nattdumpar (arenden, redovisning, hermes-zip), sju rullande platser.
Dekryptering: gpg --batch --passphrase-file backup-nyckel -d dumpar-dagN.tar.gpg > paket.tar
Nyckeln ligger ALDRIG har.
