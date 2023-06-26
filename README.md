better french azerty for math, physics and german
==================================================
** MODIFIED **
	capslock 
		does not lock non letters (same behavior as english US qwerty)
		gives access to caps letters with diacritic (majuscules accentuées)
** ADDED **
	acute accent dead key
		altgr ^ (row below numbers next to letter P)
			touche avec déjà 2 diacritiques en dead key : ^ circonflexe et ¨ tréma diaeresis umlaut
			TODO amélioration possible : accent sur certaines consonnes pas seulement les voyelles (ex : ẃ en welsh)
	math & logic & physics
		/ dead key
			altgr / 	suivi de
				inequalities
					= -> ≠
					≃ -> ≄
					< -> ≮
					> -> ≯
					⩽ -> ≰
					⩾ -> ≱
				other
					o -> ø
					O -> Ø
						empty set
					h -> ℏ
						Planck constant
		TODO other equality symbols
			≈ (~)
				altgr shift ~ 	(altgr shift é)
				TODO ≃ (asymptotically equal to) ?
			altgr with some key to enable math stuff : altgr numpad . or + or - 	maybe ?
				≃
				⩽
				⩾
				congruent
				...
			NOTE that we do not want to change ~ behavior as for example ~= has defined meaning in many programming languages and is very different from "approximately equal to"
		TODO 
			∂ Partial Differential 
			U+2202
		TODO
			Newton's derivative notation
			https://en.wikipedia.org/wiki/Notation_for_differentiation#Newton's_notation
		lettres grecques
			altgr lettre -> minuscule
			altgr shift lettre -> majuscule
				follows standard greek qwerty keyboard mapping
					** lettre latine correspondante ** lorsqu'elle existe
						à noter que
						I i -> Ι ι 	(not J j)
						Y y -> Υ ι 	(not U u)
						S s -> Σ σ  (not C c) (@see particularités [σ Σ ς sigma](#sigma))
					lettres sans correspondance naturelle
						C c -> ψ Ψ
						J j -> Ξ ξ
						U u -> Θ θ
						V v -> Ω ω
						w 	-> ς 	(final sigma)
				Ε ε epsilon
					altgr e correspond déjà à €, hors on ne veux pas changer la disposition par défaut
					=> altgr **shift** e
				σ Σ ς sigma, final sigma	<span id="sigma"></span>
					σ
						capslock shift s
						on réserve altgr s au ß eszett allemand
						TODO version math sans german eszett
							```
							//σ Σ ς
							1f	S		SGCap	s	S	-1	03c3	03a3	// LATIN SMALL LETTER S, LATIN CAPITAL LETTER S, <none>, GREEK SMALL LETTER SIGMA, GREEK CAPITAL LETTER SIGMA
							-1	-1	0	S	03c2		// LATIN CAPITAL LETTER S, GREEK SMALL LETTER FINAL SIGMA
							//ß Σ σ
							1f	S		SGCap	s	S	-1	00df	03a3	// LATIN SMALL LETTER S, LATIN CAPITAL LETTER S, <none>, LATIN SMALL LETTER SHARP S (German), GREEK CAPITAL LETTER SIGMA
							-1	-1	0	S	03c3		// LATIN CAPITAL LETTER S, GREEK SMALL LETTER SIGMA
							```
					Σ
						altgr shift s 	(normal)
					ς final sigma
						capslock shift c 	(**ADDED** par rapport au standard greek qwerty keyboard mapping)
				diacritics
					greek tonos, greek dialytika tonos
						**NOT included** to avoid overloading the layout
							/* where could we put them ? ¨ ? but we already added ´ (acute accent) on altgr ¨ */
					diaeresis
						applied to relevant greek letters
							ϊΪ ϋΫ
			alternative 
				lorsque pas de correspondance latine (ou correspondance approchante déjà occupée)
					lettre latine inoccupée la ** graphie la plus proche **
						Θ θ thêta theta
							=> Q
							graphie proche
							(t occupé par Τ τ tau)
							(Ϙ ϙ qoppa not included)
						Ξ ξ xi
							=> c
							(choix discutable entre Ξ ξ xi et χ Χ khi pour x, touche proche choisie bien que c == σ Σ ς sigma)
							(à noter double correspondance s et c pour σ Σ ς sigma mais on a besoin d'une touche, ς sur capslock shift c tout de même)
						χ Χ khi
							=> x
							(choix discutable entre Ξ ξ xi et χ Χ khi, graphie proche choisie)
						ψ Ψ psi
							=> v
							(pas terrible mais pas mieux)
						Ω ω	oméga omega
							=> w
							graphie minuscule proche
							(o occupé par Ο ο omicron TODO remplacer par oméga car omicron identique au o latin ?)
				double correspondance pour
						Ι ι iota
							i
							j
						Υ ι uspilon
							u
							y
				```
				15	Y		1	y	Y	-1	03c5	03a5		// LATIN SMALL LETTER Y, LATIN CAPITAL LETTER Y, <none>, GREEK SMALL LETTER UPSILON, GREEK CAPITAL LETTER UPSILON
				16	U		1	u	U	-1	03c5	03a5		// LATIN SMALL LETTER U, LATIN CAPITAL LETTER U, <none>, GREEK SMALL LETTER UPSILON, GREEK CAPITAL LETTER UPSILON
				17	I		1	i	I	-1	03b9	0399		// LATIN SMALL LETTER I, LATIN CAPITAL LETTER I, <none>, GREEK SMALL LETTER IOTA, GREEK CAPITAL LETTER IOTA
				1e	Q		1	q	Q	-1	03b8	0398		// LATIN SMALL LETTER Q, LATIN CAPITAL LETTER Q, <none>, GREEK SMALL LETTER THETA, GREEK CAPITAL LETTER THETA
				24	J		1	j	J	-1	03b9	0399		// LATIN SMALL LETTER J, LATIN CAPITAL LETTER J, <none>, GREEK SMALL LETTER IOTA, GREEK CAPITAL LETTER IOTA
				2c	W		1	w	W	-1	03c9	03a9		// LATIN SMALL LETTER W, LATIN CAPITAL LETTER W, <none>, GREEK SMALL LETTER OMEGA, GREEK CAPITAL LETTER OMEGA
				2e	C		SGCap	c	C	-1	03be	039e		// LATIN SMALL LETTER C, LATIN CAPITAL LETTER C, <none>, GREEK SMALL LETTER XI, GREEK CAPITAL LETTER XI
				-1	-1	0	C	03c2		// LATIN CAPITAL LETTER C, GREEK SMALL LETTER FINAL SIGMA
				2f	V		1	v	V	-1	03c8	03a8		// LATIN SMALL LETTER V, LATIN CAPITAL LETTER V, <none>, GREEK SMALL LETTER PSI, GREEK CAPITAL LETTER PSI
				```
		¬ "not operator" (also "not sign")
			altgr !
		exposants et indices
			cf [indices et notes](#superscript-subscript)
		set symbols
			TODO N, Z, Q, R, C ?
			∈ "element of"
				altgr shift e
			∉ "not element of"
				TODO with / dead key
			Ø "empty set" AS latin capital letter o with stroke instead of ∅ real "empty set" as the former is more likey to be included in fonts
			ø
				altgr shift o
				altgr o
			⊂, ⊃ "subset of", "superset of"
				TODO 2282	2283
			⊄, ⊅ "not subset of", "not superset of"
				TODO with / dead key
			×
				AltGr *		(µ next to enter key, not on numpad)
				TODO numpad ? require scan code and VK
	guillemets français 
		capslock <
		capslock shift < (ie. capslock >)
	·	"point médian"
		altgr .		(altgr ;)
	indices et notes <span id="superscript-subscript"></span>
		via dead keys
		superscript
			shift ² 	ou  	capslock ²
				suivi des chiffres ⁰¹²³⁴⁵⁶⁷⁸⁹
				suivi des charactères ⁺⁻⁼⁽⁾
				suivi des lettres ᵃᵇᶜᵈᵉᶠᵍʰⁱʲᵏˡᵐⁿᵒᵖ𐞥ʳˢᵗᵘᵛʷˣʸᶻ(toutes sauf q)
					TODO MSKLC does not support U+107a5  (0071	107a5	// q -> 𐞥)
				suivi de espace ˄ "Modifier Letter Up Arrowhead"
					(/!\ différent de ^ circonflexe notamment pour ne pas interférer avec l'existant : texte habituel, opérateur bit à bit XOR, bitwise XOR operator)
					TODO alternative ⌄ "Up Arrowhead" ? no does not seem to work without modifier before
		subscript
			altgr ²
				suivi des chiffres ₀₁₂₃₄₅₆₇₈₉
				suivi des charactères ₊₋₌₍₎
				suivi des lettres ₐₑₕᵢⱼₖₗₘₙₒₚᵣₛₜᵤᵥₓ (uniquement aehijklmnoprstuvx, ie manque bcdfgqwyz)
				suivi de espace ˅ "Modifier Letter Down Arrowhead"
					TODO alternative ⌄ "Down Arrowhead" ? no does not seem to work without modifier before
	ligatures
		TODO
		oe
		ae
		autres ?
	allemand
		ß
			altgr s
		* no capital ẞ (rarely used) *
		„“
			TODO guillemets allemand ?
	espagnol
		TODO via dead key comme le azerty-afnor ?
			AltGr+Eu (AltGr+H) suivi d'une lettre
		¿
			altgr ?
			TODO remove
		¡
			TODO


better french azerty for math, physics
=======================================
TODO same as former with no ß eszett on altgr s
	but instead 
		σ on: altgr s
		ς final sigma on: capslock shit s	(still also on: capslock shit c)


greek azerty
=============
based on standard greek keyboard but mapped to french azerty instead of qwerty
	
** ADDED **
	supports improvements from [better french azerty for math, physics and german]() (added part only, as capslock behavior is made to follow qwerty keyboards)
		those improvements are totally invisible if you do not care
	altgr σ 
		ς (final sigma)

** MODIFIED **
	decimal separator on numeric keypad
		. 	(instead of ,)
	TODO alt version without this

TODO 
	tonos
	dialytika tonos


TODO replace superscript & supscript letter with greek letters



@see also other interesting keyboards
=======================================
AFNOR
	[fr azerty AFNOR NF Z71-300] (https://www.boutique.afnor.org/fr-fr/norme/nf-z71300/interfaces-utilisateurs-dispositions-de-clavier-bureautique-francais/fa188960/1792) (/!\ norme payante, pas lue personnellement)
	description http://norme-azerty.fr/
	une implémentation windows https://github.com/springcomp/optimized-azerty-win/tree/main
		doc de l'implémentation https://springcomp.github.io/optimized-azerty-win/
	une implémentation linux https://github.com/Djyp/azerty_afnor