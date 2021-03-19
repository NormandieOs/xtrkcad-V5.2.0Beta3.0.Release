
Notes de mise à jour de la bêta 3.0
Bienvenue dans la version XtrackCAD V5.2.0 Beta 3.0!

La bêta 3.0 a quelques améliorations fonctionnelles et quelques corrections de bogues depuis la bêta 2.1. La bêta 3.0 est destinée à être un prélude à une version GA. Nous avons uniquement l'intention d'ajouter des correctifs et non des améliorations fonctionnelles à ce stade.

La version V5.2 a commencé comme de simples améliorations fonctionnelles de longue date, comme les images d'arrière-plan. L'idée était de lancer toutes les modifications de l'interface utilisateur de la version V6 GTK3. Mais en cours de route et en raison de certains sabbatiques pour les développeurs, les choses ont continué à être ajoutées et bricolées. Enfin, les principales améliorations de l'interface utilisateur que vous verrez ont été cartographiées au cours des six derniers mois et nous avons donc également une amélioration progressive de l'interface utilisateur.

Martin et Dave et Adam, vos développeurs bénévoles.

PS Le journal des modifications complet est un fichier dans le dossier de téléchargement XtrkCAD sous CHANGELOG.md

Avertissement aux utilisateurs
Veuillez noter que ce logiciel contient des bogues. Ne l'utilisez pas si cela vous dérange. Tous les logiciels contiennent des bogues, bien sûr, mais les logiciels bêta sont notre chance de trouver et de supprimer autant d'entre eux que possible avant de les libérer pour tous les utilisateurs. Vous, nos partenaires de test bêta dans cette entreprise, aidez en vous exposant au risque d'échec et en nous faisant ensuite savoir comment cela s'est passé. Ceci est vital, vous devez nous faire savoir quand les choses ne se passent pas comme prévu, ou si elles se produisent (nous savons donc que quelqu'un teste).

Faites des sauvegardes! S’il vous plaît. Les fichiers écrits par XTrackCAD 5.2.0 sont versionnés pour être lus uniquement par 5.2.0, mais il peut également lire les fichiers des versions antérieures. Si vous rencontrez des problèmes, veuillez nous contacter, nous pourrons peut-être vous aider, mais pas si vous n'avez pas effectué de sauvegarde.

Nous corrigerons les bogues importants que vous rencontrez en publiant des mises à jour bêta périodiques. Nous ne pouvons pas changer le code si ce à quoi vous vous attendez est impossible ou briserait ce que nous essayons de réaliser globalement, mais nous promettons que nous examinerons toutes vos contributions aussi attentivement que possible. Évidemment, si le programme échoue d'une manière ou d'une autre, faites-le nous savoir. Mais faites-nous également savoir quand vous ne pouvez pas régler les choses ou que la façon dont les choses semblent fonctionner semble irrationnelle. Exercez également la documentation (lisez le manuel d'aide lorsque vous êtes bloqué - il y a maintenant un raccourci F1 pratique vers les pages de la fonction actuelle ...)

Pour signaler des bogues, veuillez utiliser la page de rapport de bogues de SourceForge https://sourceforge.net/p/xtrkcad-fork/bugs/

Pour discuter de la bêta, veuillez utiliser le forum des utilisateurs https://xtrackcad.groups.io/g/main/topics

Remarques sur la philosophie de l'interface utilisateur V5.2
XtrackCAD est un produit vétéran. Conçu dans un monde d'interfaces graphiques vectorielles UNIX, puis porté sur Windows également, son fonctionnement a été optimisé pour une ère matérielle où le redessiner complet de l'écran était une opération douloureuse. Le déplacement d'objets autour de la pièce nécessitait une simplification du dessin et une approche de réécriture. Le style d'interface utilisateur chic à l'époque était très modal - vous avez choisi un outil dans une barre d'outils, puis vous l'avez utilisé en sélectionnant une cible - Pensez à Photoshop. Chaque commande / outil était un monde en soi avec des règles différentes à maîtriser. L'apprentissage du programme a nécessité beaucoup de pratique, mais vous a récompensé avec de nombreux raccourcis et fonctions qui nécessitaient une séquence d'actions.

Maintenant que nous sommes en 2020, notre matériel est beaucoup plus puissant même si nous avons une machine vieille de quelques années. Nous sommes habitués à des UI plus réactives et immersives qui tentent d'anticiper l'utilisateur et de le guider. De nombreuses interfaces utilisateur ont un style plus «choisir un objet, puis effectuer diverses actions». En partie par nécessité, XTrackCAD semblera familier à ses utilisateurs fidèles et fonctionnera en grande partie de la même manière pour eux, mais l'un des principaux objectifs des améliorations de l'interface utilisateur a été d'essayer de combler le fossé sémantique vers les programmes grand public couramment utilisés d'aujourd'hui pour lisser le sur- expérience de la rampe. La prévisibilité est la clé - puis-je comprendre ce qui va se passer avant de le faire et ainsi apprendre en explorant? Suis-je capable de naviguer plus facilement entre les fonctions communes et est-ce que les objets que je vois se comportent de la manière que j'attendais?

Nous avons passé au peigne fin les suggestions des utilisateurs, repensé à nos propres premières expériences, réalisé des enquêtes sur d'autres produits de conception graphique et interrogé directement les utilisateurs sur les choix que nous pourrions faire. Nous avons également examiné tous les commentaires que nous avons pu trouver en ligne (bons ou mauvais) des modélisateurs ferroviaires / ferroviaires. Cela nous a amenés à comprendre que les nouveaux utilisateurs pensaient à XTrackCAD comme un ensemble de pistes en attente d'être assemblés et qu'ils étaient déroutés par des choses simples - pourquoi dois-je sélectionner les aiguillages différemment de la piste flexible ? Pourquoi le programme est-il si difficile sur la façon dont les pistes s'alignent - ne devrait-il pas simplement se joindre ? Pourquoi certaines de mes commandes affectent-elles les objets que je ne vois même pas à l'écran ? Pendant ce temps, les utilisateurs avancés avaient d'autres préoccupations.Pourquoi ne puis-je pas dessiner des objets précis comme dans une «vraie» CAO ? Pourquoi ne puis-je pas utiliser Cornu pour plus que rejoindre ? Pourquoi les fichiers de paramètres sont-ils si difficiles à choisir ?

Il y a plusieurs choses que nous n'avons pas faites dans l'interface utilisateur car elles auraient été trop complexes sur une base d'interface graphique Windows / GTK divisée - celles-ci devront attendre la V6. Mais dans l'ensemble, nous espérons que les nouveaux utilisateurs trouveront la V5.2 plus accessible, tandis que les utilisateurs expérimentés découvriront des fonctionnalités améliorées qu'ils peuvent utiliser (même celles qui ont toujours existé mais qui étaient bien cachées).

Notre critère est donc le suivant -> avoir à utiliser moins de clics pour effectuer des tâches courantes, rendre les actions restantes plus précises et avec moins d'effets secondaires. Nous souhaitons prendre en charge la création de pistes faciles à assembler ainsi que la création de dessins de haute précision. Pour permettre une meilleure annotation et un meilleur traçage des emplacements réels, pour encourager une plus grande production de pièces réutilisables en facilitant leur recherche. Même si un «look» moderne attendra la personnalisation du V6, nous voulions faire de notre mieux avec le framework d'interface utilisateur «classique» dont nous avons hérité debout sur les épaules des géants qui nous ont précédés.

Adam R

PS Si vous ne pouvez pas «suivre» avec la nouvelle méthode de sélection, vous pouvez revenir à la sélection «classique» avec -

Options-> Commande-> Sélectionnez Ajouter et décochez Sélectionner Aucun
Désactiver l'accrochage magnétique
Notes d'installation
Mac OS X
Mac OSX installe un package d'application que vous faites glisser dans le dossier Applications. Pour l'exécuter, vous devez d'abord avoir installé XQuartz à partir de http://www.xquartz.org . N'oubliez pas de vous connecter et de vous déconnecter après avoir installé XQuartz pour la première fois.

Sur Mojave et les versions antérieures, le programme peut ne pas fonctionner lors de la première exécution après avoir essayé de l'exécuter - Allez dans Préférences-> Sécurité et sélectionnez "Exécuter quand même".

Sur Catalina, XTrackCAD ne fonctionnera pas en double-cliquant sur l'application - Vous devez le sélectionner avec le bouton droit dans le Finder dans le dossier Applications et sélectionner "Ouvrir". L'application perd l'accès à certains dossiers à haut risque / haute sécurité, y compris les dossiers Téléchargements, Documents et Musique - si vous avez du matériel que vous devez utiliser dans ces zones, copiez-les dans d'autres dossiers.

les fenêtres
XTrackCAD v5.2 est une application 32 bits. Pour prendre en charge les nouvelles fonctionnalités, le package est livré avec trois DLL. Deux d'entre eux (zlib et zip) nécessitent vcruntime140.dll, qui n'est pas inclus dans le package. Vous devrez donc obtenir une version 32 bits de cette DLL et l'installer dans votre chemin.

Essayez https://www.microsoft.com/en-US/download/details.aspx?id=48145

Linux
L'installation du paquet Debian (xtrkcad-setup-5.2.0Beta2.0-1.x86_64.deb) ou du paquet RPM (xtrkcad-setup-5.2.0Beta2.0-1.x86_64.rpm) s'installera dans / usr / local / bin / et / usr / local / share /.
Un accès super-utilisateur sera nécessaire pour l'installer.
Sachez que vous n'appelez aucune autre installation xtrkcad existante lors de l'exécution du programme.

Le paquet debian est nouveau mais mieux intégré, et nous recommandons aux utilisateurs de distribution de type Debian de l'essayer en premier.

L'installation de l'archive shell xtrkcad-setup-5.2.0Beta2.0-1.x86_64.sh s'installera dans le répertoire courant. Vous aurez le choix d'installer les répertoires bin / et share / dans le répertoire courant ou dans un sous-répertoire (xtrkcad-setup-5.2.0Beta2.0-1.x86_64 /).
Vous devez définir la variable d'environnement XTRKCADLIB à l'emplacement du répertoire share / xtrkcad:
- export XTRKCADLIB = pwd/ share / xtrkcad ou
- export XTRKCADLIB = pwd/xtrkcad-setup-5.2.0Beta2.0-1.x86_64/share/xtrkcad

Pour exécuter xtrkcad, vous devrez l'exécuter à partir d'une fenêtre de terminal. Pour l'archive shell, le répertoire bin / installé doit être dans votre chemin ou le chemin vers le répertoire bin / doit être spécifié.
Nous travaillons à l'intégration de xtrkcad avec le système de menus.

webkitgtk n'est pas utilisé pour afficher l'aide. À la place, votre navigateur système sera utilisé.

=================================================== =================================================== ==

Notes de version de XTrackCAD 5.2.0
Ce fichier contient des instructions d'installation et des informations à jour concernant XTrackCad.

Contenu
À propos de XTrackCad
Informations sur la licence
Installation
Mise à niveau à partir de versions antérieures
Bugs corrigés
Construction
Où trouver du soutien
À propos de XTrackCad
XTrackCad est un puissant programme de CAO pour la conception de schémas de chemin de fer miniature.

Quelques points forts:

Facile à utiliser.
Prend en charge toutes les échelles.
Fourni avec des bibliothèques de paramètres pour de nombreuses marques d'aiguillages populaires, ainsi que la possibilité de définir les vôtres.
Calcul automatique de la courbe de servitude (transition en spirale).
Fichiers d'aide étendus et mode de démonstration de clip vidéo.
Disponibilité:
XTrkCad Fork est un projet de développement ultérieur du
logiciel original XTrkCad . Voir la page d'accueil du projet à http://www.xtrackcad.org/ pour les nouvelles et les versions actuelles.

Informations sur la licence
Copier:

XTrackCad est protégé par les droits d'auteur de Dave Bullis et Martin Fischer et est licencié en tant que logiciel libre selon les termes de la licence publique générale GNU v2 que vous pouvez trouver dans le fichier COPYING.

Installation
Dépendances
XTrackCAD à partir de V5.2 dépend de certaines bibliothèques externes:

Bibliothèque de compression zlib https://www.zlib.net/
libzip pour gérer les fichiers zip https://libzip.org/
De plus sur Windows uniquement

Gestion des images FreeImage http://freeimage.sourceforge.net/
Le programme d'installation Windows, Mac et Linux est fourni avec ces bibliothèques, aucun téléchargement supplémentaire n'est donc nécessaire.

Si vous construisez à partir des sources ou n'utilisez pas le gestionnaire d'empaquetage, les bibliothèques nécessaires devront être installées à l'aide des outils d'installation du logiciel du
système d'exploitation.

les fenêtres
XTrackCad n'a été testé que sur Windows 10.

La version MS-Windows de XTrackCad est livrée en tant que programme auto-extractible /
auto-installable à l'aide du programme d'installation NSIS de Nullsoft Inc.

À l'aide de l'Explorateur Windows, recherchez le répertoire dans lequel vous avez téléchargé ou copié votre nouvelle version de XTrackCAD.

Démarrez le programme d'installation en double-cliquant sur l' icône du fichier
[xtrkcad-setup-5.2.0.exe] [] .

Suivez les étapes du programme d'installation.

L'installation vous permet de définir le répertoire dans lequel XTrackCAD est
installé. Le répertoire est créé automatiquement s'il n'existe pas déjà.

Un dossier de programme nommé XTrackCAD 5 sera créé pendant le
processus d' installation . Ce dossier contient le programme, la documentation, les
fichiers de paramètres et d' exemples. Une installation existante de versions antérieures de XTrackCad n'est pas écrasée.

Un nouveau groupe de programmes nommé XTrackCAD 5 sera créé dans le menu Démarrer.

OSX
XTrackCAD for Mac est livré en tant que package OSX auto-installable
Démarrez l'installation en double-cliquant sur l' icône de fichier
[xtrkcad-osx-5.2.0.dmg] [] .

Faites glisser le package et déposez-le dans le dossier Applications.

Vous pouvez recevoir une invite vous informant que le colis n'est pas signé. Pour l'installer quand même, accédez à la page Préférences Système et sélectionnez Sécurité et confidentialité. Appuyez sur le bouton "Installer quand même".

Si vous avez une version précédente, il vous sera demandé si vous souhaitez la remplacer ou installer une deuxième version.

Vous devrez avoir installé le niveau correct de XQuartz pour votre niveau d'OSX pour exécuter XTrackCAD sur Mac - allez sur http://www.xquartz.org/ et téléchargez puis installez le package. N'oubliez pas de vous déconnecter et de vous reconnecter (ou de redémarrer) s'il s'agit de votre première installation de xQuartz.

Une fois le package XQuartz installé, accédez à l'icône XtrkCAD dans Applications et double-cliquez dessus. On vous dira peut-être à nouveau que le programme n'est pas signé. Si tel est le cas, allez à nouveau dans Préférences système-> Sécurité et confidentialité et cliquez sur "Exécuter quand même".

Sur Catalina, vous devrez démarrer le programme en faisant un clic droit sur l'icône et en sélectionnant «Ouvrir».

Linux
XTrackCAD for LINUX est livré sous forme de fichier RPM et d'archive auto-extractible.

Si vous modifiez le package d'installation, vous devez définir la variable d'environnement XTRKCADLIB

Par exemple, si l'installation se trouve dans le répertoire / usr / local / share / xtrkcad. vous pourriez utiliser -

env XTRKCADLIB = "/ usr / local / share / xtrkcad /" xtrkcad

Installation à partir du package RPM.
Utilisez le gestionnaire de packages de votre système d'exploitation pour installer XTrackCAD.

Installation à partir de l'archive auto-extractible.
Après le téléchargement, ouvrez une ligne de commande puis exécutez en tant que root

./xtrkcad-setup-5.2.0.x86_64.sh --prefix = / usr / local --exclude-subdir
Cela installera l'exécutable dans / usr / local / bin. Un répertoire nommé
xtrkcad sera créé dans / usr / local / share et tous les fichiers y seront décompressés
.

Si vous installez XTrackCAD dans un autre répertoire, définissez la
variable d'environnement XTRKCADLIB pour qu'elle pointe vers ce répertoire.

Informations de sortie
Informations de mise à niveau
Remarque: cette version de XTrackCAD est livrée avec plusieurs nouvelles fonctionnalités
telles que des images d'arrière-plan ou des extensions de notes. Afin de prendre en charge
cette fonctionnalité, un format de fichier supplémentaire pour les fichiers de mise en page (.xtce) a été ajouté.
L'ancien format .xtc est toujours pris en charge pour la lecture et l'écriture. Ainsi, les
fichiers des versions antérieures de XTrackCAD peuvent être lus sans problème.
Les mises en page enregistrées dans le nouveau format ne peuvent pas être lues par les anciennes
versions de XTrackCAD.

Construction
Aperçu
Les instructions suivantes détaillent la construction de XTrackCAD à l'aide de CMake. CMake est un système de génération multiplateforme, disponible sur http://www.cmake.org , qui peut être
utilisé pour générer des builds pour une variété d'outils de build allant de «make» à
Visual Studio et XCode. En utilisant CMake, vous pouvez créer XTrackCAD sous Windows,
GNU / Linux et Mac OSX en utilisant le ou les outils de construction de votre choix.

Construire XTrackCAD sur GNU / Linux
Obtenez les sources actuelles de Mercurial; Je suppose qu'ils sont stockés localement dans
"~ / src / xtrkcad".
Notez que l'URL correcte pour l'accès en lecture seule à Mercurial est
http://xtrkcad-fork.hg.sourceforge.net:8000/hgroot/xtrkcad-fork/xtrkcad
Passez à la branche V5.2 en utilisant "hg update V5.2"
Créez un répertoire de construction séparé; pour ces instructions, je suppose que
votre répertoire de construction est "~ / build / xtrkcad".
Exécutez CMake à partir du répertoire de construction, en lui passant le chemin vers le
répertoire source :

$ cd ~ / build / xtrkcad
$ ccmake ~ / src / xtrkcad

Appuyez sur la touche "c" pour configurer la construction. Après quelques instants, vous verrez
quatre options à configurer: CMAKE_BUILD_TYPE, CMAKE_INSTALL_PREFIX,
XTRKCAD_USE_GTK et XTRKCAD_USE_GTK_CAIRO.

Utilisez CMAKE_BUILD_TYPE pour contrôler le type de construction. Entrez «Debug» pour une version de débogage
, «Release» pour une version de version, etc.
Utilisez CMAKE_INSTALL_PREFIX pour contrôler l'emplacement d'installation du logiciel.
Pour cet exemple, je suppose "~ / install / xtrkcad".
Utilisez XTRKCAD_USE_GETTEXT pour ajouter de nouveaux paramètres régionaux (traductions de langues). Choisissez
"OFF" pour utiliser la langue par défaut de XTrackCAD (anglais). Reportez-vous à
http://www.xtrkcad.org/Wikka/Internationalization pour plus d'informations.
Utilisez XTRKCAD_USE_GTK pour contrôler le back-end de l'interface utilisateur. Choisissez "OFF"
pour Windows, "ON" pour toutes les autres plates-formes.
Utilisez XTRKCAD_USE_DOXYGEN pour activer la production de documentation de type, fonction, etc. à
partir du code source. Nécessite doxygen si activé.
Activez si et seulement si vous avez l'intention de pirater le code.
Si vous avez apporté des modifications, appuyez à nouveau sur la touche «c» pour mettre à jour votre nouvelle configuration.
Une fois que tout est configuré à votre satisfaction, appuyez sur la touche "g" pour
générer des makefiles pour votre build.
Compilez XTrkCad en utilisant votre nouvelle version:

$ faire

Installez le nouveau binaire:

$ faire installer

Exécutez le binaire installé:

$ ~ / install / xtrkcad / bin / xtrkcad

Si XTRKCAD_USE_DOXYGEN était activé:

$ make docs-doxygen

pour créer la documentation interne. Lisez cette documentation en pointant
votre navigateur Web sur ~ / build / xtrkcad / docs / doxygen / html / index.html.

Construire XTrackCAD sur Mac OSX
Vous devrez installer les dépendances suivantes - je recommande d'utiliser
http://www.macports.org pour les obtenir:
GTK2
thème-icône-gnome
tyrolienne
Une fois les prérequis installés, les instructions de construction sont les mêmes
que pour la version GNU / Linux ci-dessus.
N'oubliez pas que pour exécuter XTrackCAD sur OSX, vous devez exécuter X11 avec
votre ensemble DISPLAY.
Construire XTrackCAD sous Windows
Obtenez les sources actuelles de Mercurial; Je suppose qu'ils sont stockés localement à
"c: / src / xtrkcad".
Notez que l'URL correcte pour l'accès en lecture seule à Mercurial est
http://xtrkcad-fork.hg.sourceforge.net:8000/hgroot/xtrkcad-fork/xtrkcad
Utilisez le menu Démarrer de Windows pour exécuter CMake (cmake-gui).
Spécifiez les répertoires source et build dans la fenêtre CMake. Vous devez
fournir un répertoire de construction en dehors de l'arborescence source - j'utilise "c: / build / xtrkcad".
Appuyez sur le bouton "Configurer" pour configurer la construction. Vous serez invité à indiquer
le type de build à générer. Choisissez votre outil souhaité - J'ai utilisé "Visual
Studio 15". Après quelques instants, vous verrez deux options à
configurer: CMAKE_INSTALL_PREFIX et XTRKCAD_USE_GTK.
Utilisez CMAKE_INSTALL_PREFIX pour contrôler l'emplacement d'installation du logiciel.
La valeur par défaut "c: / Program Files / XTrkCAD" est un bon choix.
Utilisez XTRKCAD_USE_GETTEXT pour ajouter de nouveaux paramètres régionaux (traductions de langues). Choisissez
"OFF" pour utiliser la langue par défaut de XTrackCAD (anglais). Reportez-vous à
http://www.xtrkcad.org/Wikka/Internationalization pour plus d'informations.
Utilisez XTRKCAD_USE_GTK pour contrôler le back-end de l'interface utilisateur. Choisissez "OFF"
pour Windows.
Utilisez XTRKCAD_USE_DOXYGEN pour activer la production de documentation de type, fonction, etc. à
partir du code source. Nécessite doxygen si activé.
Activez si et seulement si vous avez l'intention de pirater le code.
Si vous avez apporté des modifications, appuyez à nouveau sur le bouton "Configurer" pour mettre à jour votre nouvelle configuration.
Une fois que tout est configuré à votre satisfaction, appuyez sur le bouton "OK"
pour générer des fichiers de projet pour votre build.
Compilez XTrackCad à l'aide des nouveaux fichiers de projet. Par exemple, démarrez MSVC et
ouvrez le fichier de solution "XTrkCAD.sln" qui se trouve dans votre répertoire de construction.
Construisez le projet "BUILD_ALL" pour construire le logiciel.
Construisez le projet "INSTALL" pour installer le logiciel.
Exécutez XTrackCAD en double-cliquant sur son icône située dans le répertoire d'installation -
par exemple: c: / Program Files / XTrkCAD / bin / xtrkcad.exe.
Où trouver du soutien
Les adresses Web suivantes seront utiles pour toute question ou
rapport de bogue

La liste de diffusion Yahoo! Group http://groups.yahoo.com/projects/XTrkCad
Le site Web du projet pour le développement open source http://www.xtrackcad.org/
Le site officiel de Sourceforge http://www.sourceforge.net/groups/xtrkcad-fork/
Merci de votre intérêt pour XTrackCAD.
