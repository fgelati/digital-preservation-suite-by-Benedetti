## 1 Outils de pré-versement

* Link: http://siaf.hypotheses.org/tag/pre-versement

* Note: Le Service interministériel des Archives de France (SIAF) a initié une série de travaux sur la thématique du pré-versement d’archives sur support numérique. On entend par ce terme l’ensemble des opérations permettant de préparer un paquet à verser dans un Système d’Archivage Électronique (SAE), de manière à structurer, qualifier et garantir la qualité des données et métadonnées qui seront archivées. De la capture de l’information à son empaquetage, une série de traitements et de contrôles peuvent en effet être convoqués, qu’il s’agisse du dédoublonnage, du renommage, de la gestion des formats, de la vérification d’intégrité, du classement, de la description ou encore de l’identification des fichiers problématiques ou de la traçabilité des actions effectuées.

### 1.1 Intégrité

#### 1.1.1 Calcul d’empreintes

* Link: http://siaf.hypotheses.org/444

* Note: La première thématique à laquelle nous nous intéresserons est celle du calcul d’empreintes. Ce procédé technique, qui consiste à produire une chaîne de caractères propre à un fichier et différente à chaque modification de celui-ci, est l’un des moyens utilisés, par recalcul et comparaison des empreintes à plusieurs moments dans le cycle de vie du document, pour garantir l’intégrité de l’information dans le temps, avec d’autres procédés, comme l’horodatage. Le calcul d’empreintes peut aussi intervenir dans d’autres traitements, comme l’identification et la gestion des doublons. Nous nous concentrerons sur les outils spécialisés dans cette fonctionnalité, tout en sachant que d’autres outils, plus généralistes, la proposent également.

##### 1.1.1.1 ExactFile

* Link: http://www.exactfile.com/

* Note: ExactFileÉditeur : StudyLamp SoftwareLicence : FreewareExactFile est un outil Windows disposant d’une interface facile à prendre en main. Il permet de calculer des empreintes selon des algorithmes variés (MD5, SHA, CRC32, Adler32, GOST, RIPEMD, TIGER) sur des dossiers et fichiers. Il produit, après traitement, un manifeste qui sert à vérifier la conformité des empreintes dans le temps.

##### 1.1.1.2 FastSum

* Link: http://www.fastsum.com/

* Note: FastSumÉditeur : Kirill ZinovLicence : Logiciel payant (version d’évaluation disponible)FastSum est un outil Windows capable de calculer des empreintes en utilisant l’algorithme MD5 seulement. Il produit un rapport d’analyse servant à contrôler les empreintes dans le temps.

##### 1.1.1.3 

* Link: https://www.avpreserve.com/tools/fixity/

* Note: FixityÉditeur : AVPreserveLicence : APL2Fixity fonctionne sous Windows et Mac. En sus du calcul d’empreintes en utilisant différents algorithmes sur les dossiers et fichiers, Fixity se distingue par la possibilité de configurer des tâches de contrôle d’intégrité planifiées et de recevoir des alertes par courriel en fonction de leur succès ou de leur échec. Le manifeste n’est cependant pas directement accessible.

##### 1.1.1.4 Hasher

* Link: http://www.den4b.com/?x=products

* Note: HasherÉditeur : Furious TechnologiesLicence : CC-BY-NC-ND (version Lite et version Pro)Outil fonctionnant sous Windows, Hasher fait partie d’une suite de produits destinés à faciliter les traitements sur les fichiers bureautiques. Il dispose d’une interface assez intuitive et permet de calculer des empreintes en simultané avec plusieurs algorithmes et d’exporter le résultat obtenu, sans possibilité de vérification a posteriori.

##### 1.1.1.5 Md5Summer

* Link: http://www.md5summer.org/about.html

* Note: Md5SummerÉditeur : Luke PascoeLicence : GPLParticulièrement simple à installer et à utiliser avec une interface dédiée, MD5Summer est un outil Windows capable de calculer en MD5 les empreintes de fichiers ou de dossiers puis de les exporter dans un fichier .MD5. Ce fichier peut ensuite servir de support à des vérifications périodiques d’intégrité.

##### 1.1.1.6 HashMyFiles

* Link: http://www.nirsoft.net/utils/hash\_my\_files.html

* Note: HashMyFilesÉditeur : Nir SoferLicence : FreewareHashMyFiles se limite, sous Windows, à de la création d’empreintes avec plusieurs algorithmes (MD5, CRC32, SHA1, SHA256, SHA512) et à l’export de la liste des empreintes calculées dans un fichier. Il dispose par ailleurs d’une fonction de repérage des fichiers possédant des empreintes similaires, ce qui peut servir à identifier les doublons.

##### 1.1.1.7 JackSum

* Link: http://www.jonelo.de/java/jacksum/

* Note: JackSumÉditeur : Johann N. LöfflmannLicence : GPL2Outil Java en ligne de commande fonctionnant sur toute plate-forme, Jacksum est capable de calculer unitairement ou par dossier les empreintes des fichiers en utilisant plusieurs algorithmes. Des options de contrôle peuvent être ajoutées, et les empreintes peuvent être vérifiées a posteriori.

##### 1.1.1.8 Manifest Maker

* Link: http://manifestmaker.sourceforge.net/

* Note: Manifest MakerÉditeur : Archives nationales d’AustralieLicence : GPL3Manifest Maker est un outil en Python compatible avec toutes les plates-formes. Il permet de sélectionner des dossiers ou des fichiers et d’exporter un manifeste en .tsv contenant l’ensemble de leurs empreintes calculées en SHA512. Sa vocation première réside dans la préparation d’un lot de fichiers pour gravure sur un support optique.

##### 1.1.1.9 MD5Deep/Hashdeep

* Link: http://md5deep.sourceforge.net/

* Note: MD5Deep/HashdeepÉditeur : Jesse KornblumLicence : LibreMD5Deep et HashDeep sont une combinaison d’outils utilisables sous Windows en ligne de commande et permettant de calculer des empreintes en utilisant différents algorithmes, de produire un manifeste, puis de vérifier à nouveau les empreintes calculées.

#### 1.1.2 Copie contrôlée

##### 1.1.2.1 DataAccessioner

* Link: http://siaf.hypotheses.org/588

* Note: DataAccessioner est un outil sous licence libre (sans réutilisation commerciale) disposant d’une interface graphique et destiné à la copie contrôlée et décrite de fichiers d’un support vers un autre. Écrit en Java, il est portable sur toutes les plates-formes. Il a été développé pour la David M. Rubenstein Rare Book and Manuscript Library de l’université Duke aux États-Unis afin de copier facilement des fichiers issus d’un support CD vers des serveurs pour des opérations de classement ultérieures. Le produit est aujourd’hui maintenu dans le cadre du projet POWRR. La dernière version (v1.0.0-beta) date du 13 août 2014.

##### 1.1.2.2 Robocopy

* Note: Cet outil n'a pas été présenté dans le carnet du SIAF, mais a été rajouté car utilisé par plusieurs services d'archives.

### 1.2 Pérennité

#### 1.2.1 Identification et validation des formats de fichiers

* Link: http://siaf.hypotheses.org/676

* Note: La pérennisation de l’information numérique passe par deux étapes primordiales d’identification et de validation des formats de fichiers. Au cours de la première, on reconnaît le format et dans la seconde, on vérifie que le fichier respecte bien ses spécifications.Bien que ces deux fonctions doivent être distinguées, nous les traitons dans le même billet car beaucoup d’outils réalisent les deux, l’une à la suite de l’autre, même si certaines applications ne proposent qu’une validation des formats.Cette liste d’outils d’identification et de validation des formats n’est pas exhaustive et contient beaucoup de références à des applications « généralistes » gérant plusieurs formats de fichiers. Il existe également d’autres ressources spécifiquement dédiées à des formats en particulier (PDF1, MP3, TIFF…). Tous les outils sélectionnés sont disponibles sous licence libre (mais il en existe également sous licence propriétaire), permettent de réaliser des traitements en masse et proposent généralement des fonctionnalités en mode service. Ils peuvent être lancés en ligne de commande ou être utilisés comme composants dans d’autres applications plus larges comme des systèmes d’archivage électronique.Les étapes d’identification puis de validation des formats, se basent sur des référentiels eux-mêmes alimentés par les spécifications de ces formats. Il faut enfin noter que si ces outils sont efficaces avec les formats de fichier qu’ils répertorient, ils atteignent leurs limites avec des fichiers aux formats moins courants ou dont les spécifications ne sont pas ouvertes.

##### 1.2.1.1 CSV Validator

* Link: http://digital-preservation.github.io/csv-validator/

* Note: CSV ValidatorÉditeur : Archives nationales du Royaume-UniLicence : Mozilla Public V2CSV Validator permet de contrôler la validité d’un fichier CSV au regard d’un schéma CSV (csvs). Le schéma csvs a été défini par les Archives nationales du Royaume-Uni pour valider la forme et le contenu des fichiers au format CSV. L’application contrôle le fichier CSV par rapport à un schéma annexe, analysant des critères comme l’encodage, les chaînes de caractères autorisées ou encore des valeurs réservées. Les erreurs de validation s’affichent à la fin du traitement. L’outil fonctionne en ligne de commande ou dans une IHM dédiée.

##### 1.2.1.2 DROID

* Link: http://www.nationalarchives.gov.uk/information-management/manage-information/preserving-digital-records/droid/

* Note: DROIDÉditeur : Archives nationales du Royaume-UniLicence : New BSD licenceDROID permet d’identifier les formats de fichiers en se basant sur le référentiel PRONOM créé et maintenu à jour par les Archives nationales du Royaume-Uni. L’outil ne se contente pas de lire l’extension du fichier mais analyse la structure des fichiers pour identifier le format. Il fournit la version du format, le poids du fichier et la date de dernière modification. DROID indique quand l’extension ne correspond pas au format. De même, lorsque le fichier est corrompu et que l’identification est impossible, l’outil fait des propositions basées sur l’extension. Il dispose d’une interface graphique et peut être lancé en ligne de commande.

##### 1.2.1.3 FACILE

* Link: http://facile.cines.fr/

* Note: FACILEÉditeur : CINESLicence : LibreFACILE permet de vérifier le degré de conformité d’un fichier par rapport aux spécifications d’un format. Il informe si un fichier est valide et bien formé. L’outil est disponible en ligne via une interface web et propose des API de connexion distantes. FACILE est utilisé pour contrôler les entrées dans le SAE du CINES PAC et repose sur des composants comme Droid, ImageMagick ou Jhove. L’interface web présente également les formats utilisables pour archivage dans PAC.

##### 1.2.1.4 FIDO

* Link: https://github.com/openpreserve/fido/releases

* Note: FIDOÉditeur : OpenPreservationFoundationLicence : Apache License V2.0FIDO permet d’identifier les formats de fichiers en se basant sur le référentiel PRONOM. L’outil ne se contente pas de lire l’extension du fichier mais analyse la structure des fichiers pour identifier le format. Tout comme DROID, FIDO affiche la signature des formats dans ses résultats. L’outil est disponible en ligne de commande.

##### 1.2.1.5 FITS

* Link: http://projects.iq.harvard.edu/fits

* Note: FITSÉditeur : Université d’HarvardLicence : GNU LGPLFITS (File Information Tool Set) permet d’identifier, de valider et d’extraire les métadonnées de formats de fichiers. Il s’agit d’un outil en ligne de commande qui fournit des sorties XML contenant les différentes métadonnées identifiées. FITS est composé de plusieurs modules permettant de proposer plusieurs fonctionnalités dont l’identification et la validation des formats. Le fichier de résultat XML est décomposé en plusieurs grandes zones dont l’une répertorie les outils utilisés.

##### 1.2.1.6 Jhove

* Link: http://jhove.sourceforge.net/

* Note: JhoveÉditeur : Université d’HarvardLicence : GNU LGPLJhove permet d’identifier les formats et de valider leur conformité. Il distingue deux niveaux de contrôle dans son processus de validation : la bonne formation d’un format au regard de ses spécifications techniques et sa validité incluant des vérifications sémantiques. Les formats pris en charge sont les suivants : AIFF, GIF, HTML, JPEG, JPEG 2000, PDF, TIFF, Wave, XML et encodages ASCII et UTF-8. Une interface graphique est disponible mais Jhove peut fonctionner également en ligne de commande.Il est à noter que le volet 3 de l’étude du format PDF menée par le CINES, le SIAF et la TGIR HumaNum, consacré aux validateurs PDF, a testé Jhove (http://www.archivesdefrance.culture.gouv.fr/static/8196). D’autre part, une nouvelle version de l’outil est disponible à l’adresse suivante : http://www.digitalpreservation.gov/partners/jhove2.html

##### 1.2.1.7 Siegfried

* Link: http://www.itforarchivists.com/siegfried

* Note: SiegfriedÉditeur : Richard LehaneLicence : APL 2Siegfried ne propose qu’une identification des formats. L’outil se base sur le référentiel PRONOM et les signatures DROID. Il permet de lancer des traitements en masse, d’exporter ses résultats en XML, JSON ou CSV et de calculer des empreintes de fichiers en MD5, SHA1, SHA256 et SHA512.  Il est disponible en ligne de commande.

##### 1.2.1.8 SiardValidator 

* Link: https://adullact.net/scm/viewvc.php/siardValidator/?root=ff-toolbox

* Note: SiardValidatorÉditeur : Michel JacobsonLicence : GNU GPL V2SiardValidator permet de valider des fichiers au format SIARD. Ce dernier a été développé par les Archives fédérales Suisses pour archiver les bases de données relationnelles. L’outil, disponible en ligne de commande, permet de vérifier la bonne formation des fichiers et la cohérence sémantique des métadonnées archivées. Les résultats de la validation indiquent quelle étape de la validation a échoué en cas de problème.

##### 1.2.1.9 VeraPDF

* Link: http://verapdf.org/home/

* Note: VeraPDFÉditeur : VeraPDF ConsortiumLicence : GPL3, MPL2, CC-BY-4.0VeraPdf permet de valider des fichiers PDF/A en choisissant un profil de validation XML en rapport avec le fichier à valider. L’outil indique si le fichier a pu être validé et un fichier XML contient les résultats de la validation. Il propose une interface graphique et est porté par le projet européen PREFORMA.

#### 1.2.2 Gestion des Métadonnées

##### 1.2.2.1 Premis In Mets (PIM)

* Link: http://siaf.hypotheses.org/455

* Note: Premis in Mets, ou PIM, est une boîte à outils en ligne open source développée par le Florida Center for Library Automation (FCLA) pour la Bibliothèque du Congrès en 2009. Elle vise à faciliter la gestion des métadonnées liées à des fichiers numériques exprimées selon le dictionnaire de données PREMIS (PREservation Metadata : Implementation Strategies) et encapsulées dans un fichier répondant au standard METS (Metadata Encoding and Transmission Standard). Ces métadonnées sont généralement structurées dans un fichier XML.

##### 1.2.2.2 BagIt

* Link: https://tools.ietf.org/html/draft-kunze-bagit-16

#### 1.2.3 Préparation des paquets à archiver

##### 1.2.3.1 Archifiltre

* Link: https://archifiltre.io/

* Note: Outil développé dans le cadre des EIG par le ministère des affaires sociales, permet d'explorer via navigateur web des arborescences.

##### 1.2.3.2 Octave

* Link: https://francearchives.fr/fr/article/88482499

* Note: OCTAVE permet d’importer une arborescence de fichiers, tirée d’un serveur, d'un disque dur ou d’un support amovible. (Fork de Docuteam Packer)

##### 1.2.3.3 Pastis

* Link: http://pastis.cines.fr/

* Note: Pastis est un outil en cours de développement par le CINES pour générer des profils d'archivage en SEDA 2.1

##### 1.2.3.4 ReSIP

* Link: https://www.programmevitam.fr/pages/ressources/resip/

* Note: L’application ReSIP, basée sur la bibliothèque sedalib, permet de construire et manipuler des structures arborescentes d’archives, d’en éditer les métadonnées, de les importer et exporter sous la forme de SIP, sous la forme de hiérarchie disque ou encore sous forme csv pour les plans de classement.

##### 1.2.3.5 SHERPA

* Link: https://francearchives.fr/fr/article/88482498

* Note: SHERPA (Service Hébergé pour la Rédaction de Profils d'Archivage), est un outil collaboratif proposé par les Archives de France pour permettre la rédaction de profils d'archivage conformes au standard d'échanges de données pour l'archivage (SEDA).

#### 1.2.4 Conversion des formats de fichiers

* Link: http://siaf.hypotheses.org/685

* Note: L’archivage électronique nécessite de sélectionner des formats garantissant la lisibilité et l’intelligibilité des informations contenues par les fichiers sur le long terme. Outre leur identification et leur validation, il peut donc être nécessaire de convertir les formats de fichiers dans des équivalents jugés plus pérennes que les originaux.Au vu de la grande diversité des formats existants, il n’est pas possible de proposer des outils pour l’ensemble des types de fichiers que l’archiviste pourrait rencontrer. Le présent billet présente quelques solutions en mesure de répondre à certains besoins en bureautique, dans le domaine du multimédia et celui des fichiers 3D.

##### 1.2.4.1 Csv2siard

* Link: http://kost-ceco.ch/cms/index.php?csv2siard_de

* Note: Csv2siardÉditeur : Koordinationsstelle für die dauerhafte archivierung elektronischer unterlagenLicence : GNU V2Csv2siard permet de convertir des fichiers CSV en fichiers au format d’archivage des bases de données relationnelles SIARD. Le processus vérifie la syntaxe SQL et il est donc nécessaire de respecter les spécifications de cette norme dans le choix des noms de tables (accents, espaces…). L’application est disponible en ligne de commande ou dans une interface dédiée et en allemand.

##### 1.2.4.2 DraftSight

* Link: http://www.3ds.com/fr/produits-et-services/draftsight/

* Note: DraftSightÉditeur : Dassault SystèmesLicence : FreewareDrafSignt est une application qui permet de créer, d’éditer et de visualiser des fichiers DWG et DXF. Il est en mesure d’ouvrir et de manipuler des fichiers créés à partir de plusieurs outils différents dans les formats précités. Le programme présente un intérêt pour la pérennisation parce qu’il supporte de nombreuses versions des deux formats DWG et DXF, permettant des exports dans les deux sens et vers des formats de représentation de type image et PDF. Il peut être utilisé pour visualiser des fichiers anciens et les convertir.

##### 1.2.4.3 Excel Archival Tool

* Link: https://github.com/mcgrory/ExcelArchivalTool

* Note: Excel Archival ToolÉditeur : Université du MinnesotaLicence : GNU GPL V3Excel Archival Tool est un outil qui permet de convertir des fichiers XLS dans d’autres formats sans passer par Microsoft Excel lui-même. Les formats de conversion sont CSV, PNG, TXT et HTML. L’application propose une interface graphique et peut être utilisée en ligne de commande.

##### 1.2.4.4 FFMPEG

* Link: https://www.ffmpeg.org/

* Note: FFMPEGÉditeur : Projet FFmpegLicence : GNU GPLFFMPEG constitue une puissante collection d’outils donnant la possibilité de gérer des flux audio et vidéo. Parmi ces traitements, FFMPEG permet en particulier de réaliser des conversions, en ligne de commandes.D’autres outils avec interface graphique se basent sur FFMPEG. C’est par exemple le cas de WinFF qui permet d’effectuer des traitements par lot sur des fichiers (http://winff.org/html_new/).

##### 1.2.4.5 Image Magick

* Link: http://www.imagemagick.org/script/index.php

* Note: Image MagickÉditeur : ImageMagick Studio LLCLicence : GNU GPLImage Magick est un puissant outil de traitements d’images (conversion, export de métadonnées, rotation, réduction, zoom, bordure, redimensionnement…) qui propose des conversions de fichiers au format image. La conversion de format et l’identification de métadonnées sont très riches.

##### 1.2.4.6 ODF Converter

* Link: http://odf-converter.sourceforge.net/index.html

* Note: ODF ConverterÉditeur : ODF Converter TeamLicence : BSD like licenceL’outil permet de convertir des fichiers au format Microsoft OpenXml en OpenDocument. Ses traitements disponibles en ligne de commande transforment un fichier OpenXml en ODF ou inversement et valident le résultat final.

##### 1.2.4.7 OpenOffice

* Link: https://openoffice.apache.org/

* Note: OpenOfficeÉditeur : Fondation ApacheLicence : GNU LGPL3OpenOffice est une suite bureautique permettant de créer, d’éditer et de visualiser des fichiers dans des formats bureautiques, de type OpenDocument ou Microsoft Office. En plus des conversions dans des formats pérennes comme OpenDocument, elle propose des exports en PDF et PDF/A. Un mode serveur et des API de connexion sont également disponibles, ce qui donne la possibilité à d’autres applications de s’appuyer sur ses services, notamment de conversion de formats.

##### 1.2.4.8 PdfCreator

* Link: http://download.pdfforge.org/download/pdfcreator/PDFCreator-stable

* Note: PdfCreatorÉditeur : PDF ForgeLicence : GNU GPLPDFCreator est une imprimante virtuelle qui permet de convertir des fichiers imprimables en fichier PDF. L’utilisateur dispose de plusieurs fonctions de paramétrage proposées par l’outil pour choisir la version désirée du format. Il est de même possible d’ajouter certaines métadonnées au moment du traitement. PDFCreator est compatible avec une très grande variété de formats de fichiers en entrée car il s’utilise comme une imprimante à l’intérieur d’applications bureautiques.

##### 1.2.4.9 XENA

* Link: http://xena.sourceforge.net/

* Note: XenaÉditeur : Archives nationales d’AustralieLicence : GPL 3Xena est un outil capable d’identifier les formats et de les convertir. Il propose deux formes de traitement. Le mode « normalisation » permet de convertir les fichiers automatiquement vers des formats déterminés de façon préalable comme plus pérennes et de les empaqueter dans un format « Xena » pour être lus dans le visualiseur fourni dans l’application. Le mode « migration » consiste à effectuer une conversion automatique vers des formats pérennes sans empaquetage avec des métadonnées « Xena ». L’identification faite au préalable ne se base pas uniquement sur l’extension du fichier. Xena est un composant de la plateforme DPSP développée par les Archives nationales d’Australie.

##### 1.2.4.10 XnConvert

* Link: http://www.xnview.com/fr/

* Note: XnConvertÉditeur : Pierre-Emmanuel GougeletLicence : GratuicielXnConvert permet de convertir des images par lot, tout en combinant plusieurs critères de traitement. L’outil est un composant de la suite XnView et propose certaines fonctionnalités intéressantes comme une interface de visualisation des fichiers, des formulaires de modification des métadonnées associées ou l’application d’actions sur les données (rotation, compression…). Le site de l’éditeur mentionne la grande compatibilité du logiciel avec le support de 500 formats.

### 1.3 Classement et tri

#### 1.3.1 Explorer une arborescence

##### 1.3.1.1 Archifiltre

* Link: https://archifiltre.io/

* Note: Outil développé dans le cadre des EIG par le ministère des affaires sociales, permet d'explorer via navigateur web des arborescences.

##### 1.3.1.2 Pir.exe

* Link: https://pir.fr.softonic.com/

* Note: Cet outil n'a pas été présenté dans le carnet du SIAF, mais a été rajouté car utilisé par plusieurs services d'archives.

##### 1.3.1.3 WinDirStat

* Link: https://windirstat.net/

* Note: WinDirStat est un visualiseur de statistiques d'utilisation de disque et un outil de nettoyage pour différentes versions de Microsoft Windows.

#### 1.3.2 Renommage de fichiers

* Link: http://siaf.hypotheses.org/544

* Note: Le renommage en masse des fichiers avant la constitution du paquet fait partie des besoins qui sont le plus souvent évoqués par les archivistes qui se sont confrontés à des versements d’archives numériques sous la forme de fichiers bureautiques ou de courriels. Cette action, qui consiste à modifier en partie ou totalement le nom d’un fichier, répond en général à deux impératifs distincts :un impératif technique, qui réside dans la nécessité de formater les noms pour réduire le risque d’erreur dans les traitements (problèmes d’encodage des caractères spéciaux, contraintes liées à la longueur du chemin d’accès au fichier…).un impératif fonctionnel, qui réside dans la volonté de certains archivistes de faire porter une information intellectuelle dans le nom (producteur, date, cote…) comme une métadonnée minimale, tout en conservant le nom originel du fichier.

##### 1.3.2.1 Ant Renamer

* Link: https://antp.be/software/renamer/fr

* Note: Renommage de lots et remplacement de caractères multiples MAIS peu intuitif

##### 1.3.2.2 Bulk Rename Utility

* Link: http://www.bulkrenameutility.co.uk/Main_Intro.php

* Note: Bulk Rename UtilityÉditeur : Simson L. GarfinkelLicence : FreewareOutil disposant d’une interface et fonctionnant sous Windows, Bulk Rename Utility permet de sélectionner, en appliquant des filtres, des fichiers dans une arborescence puis de renommer cette sélection en masse. Les différentes étapes du traitement passent par des demandes de validation. Les possibilités de renommage sont pléthoriques, et la richesse du logiciel peut nuire à sa prise en main.

##### 1.3.2.3 Faststone

* Link: https://www.faststone.org/

* Note: Outil de visualisation avec une fonction de renommage – utile

##### 1.3.2.4 FreeCommander XE

* Link: http://freecommander.com

* Note: FreeCommander XEÉditeur : Marek JasinskiLicence : FreewareFreeCommander n’est pas qu’un outil de renommage, mais plutôt un explorateur de fichiers rappelant les caractéristiques de l’explorateur Windows 98, avec de nombreux espaces fenêtrés. Ce logiciel est capable d’effectuer des recherches, de dédoublonner, d’appliquer des filtres et de renommer les fichiers.

##### 1.3.2.5 Personal Renamer

* Link: http://personalrenamer.blogspot.fr/

* Note: Personal RenamerÉditeur : BalisteorLicence : GPLPersonal Renamer est un outil fonctionnant sous Windows et disposant d’une interface. Il permet de sélectionner des fichiers, d’appliquer des filtres et de renommer les fichiers tout en gardant une copie de secours en cas de problème. Cependant, le manque de possibilités de validation durant les différentes étapes du traitement peut favoriser les problèmes dus à de mauvaises manipulations.

##### 1.3.2.6 Remove empty directories

* Link: https://www.jonasjohn.de/red.htm

* Note: Détection des répertoires vides et suppression – facile et pratique

##### 1.3.2.7 ReNamer

* Link: http://www.den4b.com/products/renamer

* Note: Outil simple et paramétrable – simple d’utilisation

##### 1.3.2.8 THE Rename

* Link: https://github.com/hervethouzard/THE-Rename

* Note: THE RenameÉditeur : Hervé ThouzardLicence : FreewareOutil Windows, THE Rename propose l’ensemble des fonctionnalités attendues d’un outil de renommage, en se basant principalement sur le traitement des préfixes et des extensions.

##### 1.3.2.9 Vrenamer

* Link: http://vrenamer.com/

* Note: VrenamerÉditeur : Carlos VerdierLicence : GPL3Outil Java fonctionnant sur toutes les plates-formes, Vrenamer est peut-être l’outil le plus performant de cette liste (qui n’est pas exhaustive). Simple à utiliser, il permet d’opérer en masse des actions de renommage ou de formatage des noms, en garantissant un certain niveau de sécurité grâce à des processus de validation, des alertes et la possibilité de revenir en arrière à tout moment. Cet outil est également capable de traitements approfondis sur les fichiers images et audio (enrichissement des métadonnées, prévisualisation intégrée). Toutes les opérations sont tracées et peuvent être rejouées à tout moment. Une vue du résultat final et le repérage des anomalies permettent d’éviter les mauvaises manipulations.

##### 1.3.2.10 XnView

* Link: https://www.xnview.com/fr/

* Note: Logiciel libre de traitement photo – renommage clair et intuitif- renomme tout type de fichier MAIS renomme uniquement dans un répertoire donné (et pas dans les sous-répertoires liés)

#### 1.3.3 Dédoublonnage

* Link: http://siaf.hypotheses.org/471

* Note: L’une des particularités du numérique réside dans sa facilité à dupliquer les informations pour répondre aux divers besoins des utilisateurs :sécuriser leur travail pour prévenir la dégradation des supports ou les mauvaises manipulations techniques pouvant endommager l’information.échanger des données entre plusieurs contributeurs sur un même document.disposer d’une version d’un document numérique dans leur propre environnement de travail…Ces opérations, qu’elles soient volontaires ou non, peuvent amener à gérer plusieurs copies d’un même fichier déposées à divers emplacements d’un support de stockage, sans que cela n’ait forcément un sens dans l’organisation intellectuelle d’une arborescence de fichiers. Pour diminuer les volumes stockés et améliorer la qualité et la pertinence des versements qui seront faits, il peut alors être intéressant de détecter les fichiers identiques pour les analyser et éventuellement leur appliquer des traitements pouvant aller jusqu’à l’élimination des doublons concernés.En ce qui concerne les besoins des archivistes qui ont à préparer un versement de données numériques désorganisées, l’étape d’identification des copies identiques et de leur dédoublonnage se révèle assez cruciale. Il existe plusieurs outils spécialisés dans cette fonction.

##### 1.3.3.1 AllDup

* Link: https://www.alldup.de/en\_download\_alldup.php

* Note: Cet outil n'a pas été présenté dans le carnet du SIAF, mais a été rajouté car utilisé par plusieurs services d'archives.

##### 1.3.3.2 Disk Ferret

* Link: http://www.diskferret.com/

* Note: Disk FerretÉditeur : Swooft SoftwareLicence : Logiciel payant disposant d’une version d’évaluation gratuiteOutil permettant d’analyser la composition de dossiers : analyse des fichiers, de leur taille, de leur date, contrôle de l’espace disponible, identification des doublons et des fichiers vides, cachés, ou temporaires. L’interface correspond à un explorateur de fichiers amélioré. Après la phase de capture des données, le résultat de l’analyse indique de manière claire les différents types de fichiers disponibles, les doublons et propose de les supprimer.

##### 1.3.3.3 Disk Analyzer Pro

* Link: http://www.diskanalyzerpro.com/index.html

* Note: Disk Analyzer ProÉditeur : Systweak SoftwareLicence : Logiciel payant disposant d’une version d’évaluation gratuiteDisk Analyzer Pro reprend les fonctionnalités nativement présentes dans les explorateurs de fichiers des systèmes d’exploitation modernes et vient les enrichir. Il permet d’analyser des dossiers, les fichiers qu’ils contiennent, d’afficher les métadonnées courantes de taille, la date de dernière modification, le format et d’identifier des doublons. Dans la même logique que d’autres produits concurrents, il affiche sous une forme graphique évoluée le résultat de son analyse.

##### 1.3.3.4 Dubfinder Duplicate Finder

##### 1.3.3.5 Duplicate Cleaner

* Link: http://www.duplicatecleaner.com/

* Note: Duplicate CleanerÉditeur : DigitalVolcano SoftwareLicence : Logiciel payant disposant d’une version d’évaluation gratuiteDuplicate Cleaner permet de détecter les doublons en proposant des filtres et des sources variées. Le mécanisme d’identification ne se base pas uniquement sur l’extension du fichier, son nom et son poids mais consiste à analyser également son train de bits. Des traitements en masse sont disponibles en fin d’analyse.

##### 1.3.3.6 Duplicate Files Finder

* Link: http://doubles.sourceforge.net/

* Note: Duplicate Files FinderÉditeur : Matthias BoehmLicence : GNU GPL V2Duplicate Files Finder permet de détecter les doublons en ne se basant pas uniquement sur l’extension, le nom et le poids des fichiers mais en analysant leur structure. Il est possible de lancer le travail sur plusieurs dossiers en même temps, tout en leur appliquant des filtres. En fin d’analyse, des traitements en masse comme la suppression des fichiers sont disponibles.

##### 1.3.3.7 Duplicate Searcher

* Link: https://duplicatesearcher.net/duplicate_searcher.aspx?lang=en

* Note: Outil simple et facile

##### 1.3.3.8 Fast Duplicate file finder

* Link: https://www.mindgems.com/products/Fast-Duplicate-File-Finder/Fast-Duplicate-File-Finder-About.htm

##### 1.3.3.9 Free Commander XE

* Link: http://freecommander.com/

* Note: Free Commander XEÉditeur : Marek JasinskiLicence : FreewareFree Commander XE est un explorateur de fichiers permettant d’effectuer des opérations de recherche, du dédoublonnage et du renommage. L’outil dispose de plusieurs espaces de travail (arborescence à gauche, vignettes à droites ou fichiers…) doit être surtout considéré comme un gestionnaire de fichiers avec des fonctions comme le repérage des doublons.

##### 1.3.3.10 Fslint

* Link: http://en.flossmanuals.net/fslint/

* Note: FslintÉditeur : Chris StackpoleLicence : GNU GPL V2Outil fonctionnant sous Linux permettant d’identifier les fichiers problématiques sur leurs supports. Il est en mesure de détecter les fichiers dupliqués, les mauvais formatages de nom et les fichiers temporaires.

##### 1.3.3.11 Hash My Files

* Link: http://www.nirsoft.net/utils/hash\_my\_files.html

* Note: Hash My FilesÉditeur : Nir SoferLicence : FreewareOutil permettant de calculer des empreintes sur des fichiers contenus dans divers dossiers sources. Ces empreintes enregistrées peuvent être réutilisées dans d’autres contextes comme l’identification de doublons. En fin de traitement, une coloration syntaxique permet de distinguer les fichiers « identiques ».

##### 1.3.3.12 Winmerge

* Link: https://winmerge.org/?lang=fr

#### 1.3.4 Réorganiser un fonds

##### 1.3.4.1 Docuteam Packer

* Link: https://www.docuteam.ch/fr/prestations/archivage-et-informatique/logiciels/

* Note: Cet outil n'a pas été présenté dans le carnet du SIAF, mais a été rajouté car utilisé par plusieurs services d'archives.

##### 1.3.4.2 Octave

* Link: https://francearchives.fr/fr/article/88482499

* Note: OCTAVE permet d’importer une arborescence de fichiers, tirée d’un serveur, d'un disque dur ou d’un support amovible. (Fork de Docuteam Packer)
