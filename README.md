# models_site_nan

## nombre d'appli (5)

	* configurations
	* contact
	* entreprise
	* testimony
	* blog

## configurations

	showcase(
		id,
		main-title: CharField, // grand titre
		img: ImageField, // Image du slider
		description: TextField,
		subtitle: CharField,
		page_id: ForeignKey,
		action: CharField, //Boutton principal
	),


	index_section_right_left (
	id,
	title: CharField,
	main-description: TextField,
	img: ImageField,
	side-title: CharField,
	side-description: TextField,
	)

	index_panel (
	id,
	img: ImageField,
	title: CharField,
	description: TextField,
	action: CharField,
	link: UrlField,
	),

	Call-to-action: CharField (
	id,
	img: ImageField,
	description: TextField,
	action: CharField,
	link: UrlField,
	)

	newsletter(
	id,
	name: CharField,
	title: CharField,
	img: ImageField,

	)

	Sponsor(
	id,
	img: ImageField,
	title: CharField
	description: TextField,
	),
	candidater (
	id,
	title: CharField,
	),

	environnement (
	id,
	img: ImageField,
	description: TextField,
	right_title: CharField,
	right_description: TextField,
	)
	admission (
	id,
	title: CharField,
	description: TextField,
	right_title: CharField,
	right_description: TextField,
	)
	campuslife (
	id,
	title: CharField,
	right-title: CharField,
	right-description: TextField,

	)

	section_sponsor(
	id,
	title1: CharField, //h1
	description1: TextField,
	subtitle1: CharField, //h2
	subdescription1: TextField,
	// inclure table table moyens_payment
	subtitle2: CharField,
	subdescription2: TextField,
	title2: CharField,
	),

	raison_de_sponsoriser(
	id,
	title: CharField,
	)

	moyens_paiement(
	id,
	img: ImageField,
	link: UrlField,
	)

	faq (
	id,
	question: TextField,
	reponse: TextField,

	)

	module (
	id,
	img: ImageField,
	title: CharField,
	description: TextField (tinyMCE),
	),


	## contact
	newsletter (
	id,
	email: CharField,
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
		img: ImageField,
		link: UrlField,
	)

	entreprise_map(
		id,
		longitude: Float,
		latitude: Float,
	)


## testimony

	testimony (
		id,
		img: ImageField,
		title: CharField,
		description: TextField
	)

## Blog

	categorie (
		id,
		title: CharField,
		img: ImageField,
		description: TextField,
	),

	article (
		id,
		title: CharField,
		img: ImageField,
		timestamp,
		categorie_id: ForeignKey //fk
		description: TextField,
		content: TextField,
		nb_vues: Integer,
		tag_id: ManyToMany, //many
	),

	tag(
		id,
		title: CharField,
	)
