animation_AV
============

TP1 animation


Dans le HTML dans le header, lier la feuille de styles CSS
<head>
	<link rel="stylesheet" href="animation_lib_VillAudrey.css" />
</head>


		Pour intégrer une animation à vos codes:
			dans votre page html ou php, sur votre balise ajouter class="nomClasse"
				<div class="deroulement"></div>

		Pour activer l'animation par un survole avec la sourie: 
			dans votre feuille css, après le nom de l'aimation ajouter :hover
				.nomAnimation:hover{
				}

		Modification sur le temps (en secondes)
			.nomAnimation:hover{
				nomPropriété 2s 0s infinite alternate backwards
			}
			Pour changer la durée de l'animation (de 0% à son 100%) modifier le 2s
			Pour changer le temps avant le départ de l'animation modifier le 0s
			Pour controler le nombre de répétition de l'animation, inscrire le nombre de fois voulu (ex.3fois):
				nomPropriété 2s 0s 3 alternate
			Pour laisser l'animation à son état de fin (100%)
				nomPropriété 2s 0s infinite alternate forwards
			Pour que l'animation s'effectue en boucle sans "retour inversé"
				nomPropriété 2s 0s infinite alternate
			Pour le "retour inversé" (0% à 100% puis 100% à 0%)
				nomPropriété 2s 0s infinite alternate backwards

				
.deroulement
	Appliquer sur un objet qui sera déformer avant d'être déroulé avec une transparence.

.etirement
	Appliquer sur un objet qui doublera de grandeur. Les contour du contenant courberons et une bordure rouge apparetra. Le texte aussi s'affichera à la fin de lanimation.

.descente
	Appliquer sur un objet qui descendera et rebondissera en tournant et disparaissant, avant de reprendre sa position initiale.
	On peux choisir la distance de chute (80px par en bas)
	30%{
		transform:translate(0px,80px) rotate(0);
	}

.ouverture:hover
	Appliquer sur un objet qu'on dois survoler pour dérouler/ouvrir.
	Pour que les animations fonctionnent on dois fournir certaines informations à la classe:
	Choisir la largeur finale de la boite
	.ouverture:hover{
		...
		width: 200px;
	}
	Après l'animation apparêt un ombre porté et le texte si voulu.

.disparetre
	Appliquer sur nimportequel objet qui disparetra et réaparetra

