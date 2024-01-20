# token_protector

Protecteur de jeton Discord

Protégez votre jeton Discord contre les accapareurs malveillants !

![DiscordTokenProtectorUI](https://github.com/azertyuiopexe/token_protector/assets/153385259/d484d499-004a-45c2-831f-3f4012194c79)


Ce projet est encore en cours de développement ! Vous pourriez être confronté à des problèmes d’instabilité !
Ce n’est en aucun cas une solution parfaite contre les accapareurs de jetons Discord. Mais cela vous protégera contre la plupart des accapareurs de jetons :

(Le plus courant) Lecture de LevelDB (depuis le début)
(Moins fréquent) Injection de script / altération du module Discord (à partir de dev-6)
(Rare) Lecture de la mémoire (à partir de dev-8)
Toute attaque ciblée contre DiscordTokenProtector peut contourner cette protection !

✔️Bonnes pratiques lors de l’utilisation de la PAO

⚠️ Démenti

DTP n’est pas affilié à Discord.
DTP n’est en aucun cas responsable de ce qui peut se passer sur votre compte Discord.
Les chances d’être résilié en utilisant DTP sont très faibles, mais gardez à l’esprit que l’utilisation d’un logiciel tiers est contraire aux conditions d’utilisation de Discord.

Fonctionnalités

✅ Protégez-vous de la plupart des accapareurs de jetons

✅ Stockez en toute sécurité votre jeton Discord dans un fichier crypté (les YubiKeys* sont prises en charge)

✅ Passez facilement d’un compte à l’autre

✅ Changez votre mot de passe Discord en un clic

✅ Vérifiez l’intégrité de votre installation Discord au lancement (BetterDiscord est pris en charge)

✅ Vérifier les scripts pour les logiciels malveillants connus (par exemple AnarchyGrabber3)

✅ Protéger le processus Discord de la lecture de mémoire / injection de code

✅ Protéger la PAO contre les attaques de falsification (protège le processus/la configuration contre les utilisateurs non autorisés)

*Sauf à partir de YubiKey NEO

Installation

Démarrer DiscordTokenProtectorSetup.exe

Choisissez entre l’installation normale et l’installation sans démarrage

Configurez-le

Qu’est-ce que ça fait ?

Voici un petit schéma de fonctionnement :
![how_does_it_work](https://github.com/azertyuiopexe/token_protector/assets/153385259/4567f1f5-869a-45ba-8281-c0ec4aabb068)

Il supprime les répertoires et de . Ces répertoires peuvent stocker votre jeton Discord (utilisé pour vous authentifier). La plupart des saisisseurs y cherchent votre jeton. Par conséquent, en supprimant ces répertoires, vous pouvez éviter de vous faire prendre.
Votre jeton Discord est stocké dans un conteneur sécurisé crypté avec AES-256.Local StorageSession Storage%appdata%\Discord

Crédit
Discorde
Ocornut pour ImGui
Nlohmann pour la bibliothèque JSON
CryptoPP (en anglais seulement)
Stevemk14ebr pour Polyhook v2
