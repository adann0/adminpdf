# adminpdf

Simple index/backup for my favorite resources.

## Politiques (Legal Terms)

- https://www.ssi.gouv.fr/entreprise/reglementation/protection-des-systemes-dinformations/la-politique-de-securite-des-systemes-dinformation-de-letat-pssie/

## Referentiel (Technical)

- Admin : https://www.ssi.gouv.fr/administration/guide/referentiel-dexigences-de-securite-pour-les-prestataires-dintegration-et-de-maintenance-de-systemes-industriels/
- Pentesters : https://www.ssi.gouv.fr/administration/qualifications/prestataires-de-services-de-confiance-qualifies/referentiels-exigences/

## More Precise Infos

- https://www.ssi.gouv.fr/administration/bonnes-pratiques/
- https://www.ssi.gouv.fr/administration/guide/securiser-ladministration-des-systemes-dinformation/
- https://www.ssi.gouv.fr/administration/guide/recommandations-de-securite-relatives-a-un-systeme-gnulinux/
- https://www.ssi.gouv.fr/administration/guide/profils-de-protection-pour-les-systemes-industriels/

## User

"Lorsque les systèmes d’information traitent d’informations sensibles, les terminaux permettant d’y accéder doivent impérativement être dédiés et avoir fait l’objet d’une évaluation de sécurité."

"Le stockage amovible ainsi que le stockage interne du terminal doivent être chiffrés par l’utilisation d’une solution de chiffrement robuste."

"Pour éviter toute indiscrétion lors de déplacements, notamment dans les transports ou les lieux d’attente, un filtre de confidentialité doit être positionné sur chaque écran."

"Pour les besoins spécifiques d’authentification aux portails captifs, l’entité peut choisir de déroger à la connexion automatique en autorisant une connexion à la demande ou maintenir cette recommandation en encourageant l’utilisateur à __utiliser un partage de connexion sur un téléphone mobile de confiance.__"

- https://www.ssi.gouv.fr/administration/guide/guide-dhygiene-informatique/
- https://www.ssi.gouv.fr/administration/guide/recommandations-de-securite-relatives-aux-ordiphones/

## Admin

"Interdire l’accès à Internet depuis les postes ou serveurs utilisés pour l’administration du système d’information."

"Fortement recommandé d’établir un tunnel VPN IPsec entre le poste nomade et une passerelle VPN IPsec mise à disposition par l’entité. Pour garantir un niveau de sécurité optimal, ce tunnel VPN IPsec doit être automatiquement établi et ne pas être débrayable par l’utilisateur, c’est-à-dire qu’aucun flux ne doit pouvoir être transmis en dehors de ce tunnel."

"Le poste d’administration doit être géré par l’entité – ou à défaut un prestataire man- daté. En aucun cas l’utilisation d’un équipement personnel ne doit être tolérée pour l.’administration d’un SI."

3 niveaux (du meilleur en sécurité au moins bon) :
- un poste d’administration dédié (non connecté a internet, mais connecté au reseau local), et un poste bureautique dédié (non connecté au reseau local, mais connecté a internet);
- un poste d’administration multi-niveaux (on parle ici d'un ordinateur dont l'objectif est d'avoir 2 virtual machine avec un "noyau durci et évalué" ; une machine virtuelle s'occupera de la SI bureatique, l'autre de l'administration - il est interdit d'avoir uniquement 1 vm avec l'os hote executant des taches bureautique ou admin) ;
- un poste d’administration avec accès distant à un SI bureautique (se referer a ce guide dans ce cas pour les bonnes pratiques https://www.ssi.gouv.fr/administration/guide/securiser-ladministration-des-systemes-dinformation/).

Voir : SELinux, AppArmor, durcissement du noyau
