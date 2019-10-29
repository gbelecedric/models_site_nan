# models_site_nan

## nomnbre d'appli

* configurations
* contact
* entreprise
* testimony
* blog

## configurations
  showcase(
    id,
    main-title, // grand titre
    img, // Image du slider
    description,
    subtitle,
    page_id,
    action, //Boutton principal
  ),
  
  
  index_section_right_left (
	  id,
    title,
    main-description,
    img,
    side-title,
    side-description,
  )

index_panel (
	id,
	img,
	title,
	description,
	action,
  link,
),

Call-to-action (
	id,
	img,
	text,
	button,
)

newsletter(
	id,
	name,
	title,
	img,
  
) 

Sponsor(
	id,
	img,
	title
	description,
),
candidater (
	id,
 	title,
	),

environnement (
	id,
	img,
	description,
	right_title,
	right_description,
)
admission (
	id,
	title,
	description,
	right_title,
	right_description,
)
campuslife (
	id,
	title,
	right-title,
	right-description,

)

section_sponsor(
	id,
	title1, //h1
	description1,
	subtitle1, //h2
	subdescription2,
		// inclure table table moyens_payment
	subtitle2,
	subdescription2,
	title2,	
),

raison_de_sponsoriser(
	id,
	title,
)

moyens_paiement(
	id,
	img,
	link,
)

faq (
	id,
	question,
	reponse,

)

module (
	id,
	img,
	title,
	description (tinyMCE),
),


## contact
newsletter (
	id,
	email,
	),
  

 form_candidature (
	id,
	nom,
	prenoms,
	email,
	telephone,
	)
  

form_sponsor(
	id,
	entreprise,
	email,
	telephone,
	message,
),


  
## entreprise

entreprise_index_info(
	id,
	email,
	contact1,
	contact2,
)

entreprise_date_creation(
	id,
	date
)

entreprise_social(
	id,
	img,
	link,
)

entreprise_map(
	id,
	longitude,
	latitude,
)


## testimony
	
testimony (
	id,
	img,
	title,
	description
)

## Blog

categorie (
	id,
 	title,
	img,
	description,
),

article (
	id,
	title,
	img,
	timestamp,
	categorie_id //fk
	description,
	content,
	nb_vues,
	nb_commentaires,
	tags, //many
),

tag(
	id,
	title,
)
