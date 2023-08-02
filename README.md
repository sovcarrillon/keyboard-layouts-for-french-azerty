keyboard layouts for Windows



better french azerty for math, physics and german
==================================================
** MODIFIED **
	capslock 
		does not lock non letters (same behavior as english US qwerty)
		gives access to caps letters with diacritic (majuscules accentuées)
** ADDED **
	acute accent dead key <span id="#acute-accent">§</span>
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
				σ Σ ς sigma, final sigma	<span id="sigma">§</span>
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
					tonos (greek tonos)
						´ (acute accent) suivi d'une lettre grecque pouvant porter le tonos (ώάήέίύόΏΆΉΈΊΎΌ)
						@see [#acute-accent][]
							c'est à dire :
							altgr ^ 	*suivi de* 	altgr lettre
													altgr shift lettre
					greek dialytika tonos (greek dialytika tonos)
						on remplace ^ (circonflexe, circumflex) par dialytika tonos ΅
						^ (acute accent) suivi d'une lettre grecque pouvant porter le dialytika tonos (ΐΰ)
					diaeresis
						applied to relevant greek letters
							ϊΪ ϋΫ
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
	indices et notes <span id="superscript-subscript">§</span>
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
	TODO
		dead keys + space
			also inserts space after the raw dead key
			is it possible ?
			is it even desirable ?

[#acute-accent]: #acute-accent
[#superscript-subscript]: #superscript-subscript

better french azerty for math, physics
=======================================
TODO same as former with no ß eszett on altgr s
	but instead 
		σ on: altgr s
		ς final sigma on: capslock shit s	(still also on: capslock shit c)


greek azerty
=============
letters based on standard greek keyboard but mapped to french azerty instead of qwerty
	
** ADDED **
	supports improvements from [better french azerty for math, physics and german][] (added part only, as capslock behavior is made to follow qwerty keyboards)
		those improvements are totally transparent if you do not care
		TODO replace superscript & supscript letter with greek letters
	altgr σ 
		ς (final sigma)

** MODIFIED ** <span id="#greek-modified">§</span>
	decimal separator on numeric keypad
		. 	(instead of ,)
		TODO alt version without this
	TODO \` (accent grave) totalement remplacé par tonos
				how do we output backticks now though ???
	^ (accent circomflexe à droite du P) totalement remplacé par dialytika tonos

** INFO **
	non letter keys are thoses displayed on french azerty except for @see [#greek-modified][]
	TODO tonos produit par \` (accent grave) suivi d'une lettre
		altgr 7 *puis* lettre
	dialytika tonos produit par 
		^ (accent cironflexe à droite du P) *puis* lettre
			^ reste accessible via altgr 9
		shift w
			clavier grec standard
	q
		q -> ;
		Q -> :
		clavier grec standard
TODO 
	alt : une seule touche pour
		tonos
		diaeresis
			shift tonos
		dialytika tonos
			altgr tonos
		(à gauche du L sur le clavier grec standard)
		sur ^ ¨ ? signifie inconsistance avec better azerty


[#greek-modified]: #greek-modified
[better french azerty for math, physics and german]: #better-french-azerty-for-math-physics-and-german



korean azerty
==============
functions a bit differently: uses an IME Input Method Editor (like T9 for text message on old mobile phones)
on Windows we can keep using default IME while only changing the keyboard layout
	but changing this setting can only be done directly in the **registry**
	sources
		https://stackoverflow.com/questions/44122327/msklc-under-windows-10-create-custom-keyboard-layout-which-supports-ime-input
		https://www.reddit.com/r/LearnJapanese/comments/6qojbi/for_azerty_keyboard_users_how_to_set_up_microsoft/
		https://www.reddit.com/r/LearnJapanese/comments/f2x6mh/tip_use_ime_under_windows_with_a_nonus_keyboard/
	regedit
		HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Keyboard Layouts
			\[LOCALE_ID]
				fr-FR == 0000040c (see \HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Keyboard Layout\DosKeybCodes )
				en-US == 00000409 (		or msklc .klc files)
				ko-KR == 00000412
				\Layout File
					change dll to appropriate keyboard layout dll
						default for korean is KBDUS.DLL
						for french azerty
							KBDFR.DLL
								works almost perfectly but can't access to "?," quickly as it is used by "ㅡ"
								TODO standard azerty with M and ",?" swapped
						or use custom: [mklc keyboard ID].dll
							can be found under LOCALE_ID starting with an "a"
		**USELESS hence untested** but might be useful ? some reddit answer said to do that for japanese
			HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\i8042prt\Parameters
				\LayerDriver XXX
					change dll to appropriate keyboard layout dll
					**LayerDriver KOR** default is kbd101a.dll
		then **reboot**




@see also other interesting keyboards
=======================================
AFNOR
	[fr azerty AFNOR NF Z71-300] (https://www.boutique.afnor.org/fr-fr/norme/nf-z71300/interfaces-utilisateurs-dispositions-de-clavier-bureautique-francais/fa188960/1792) (/!\ norme payante, pas lue personnellement)
	description http://norme-azerty.fr/
	une implémentation Windows https://github.com/springcomp/optimized-azerty-win/tree/main
		doc de l'implémentation https://springcomp.github.io/optimized-azerty-win/
	une implémentation Linux https://github.com/Djyp/azerty_afnor

Korean IME with romaja support
	Nalgaeset Hangul Input System
	http://moogi.new21.org/en/ngs/index.htm

chrome input tool extension
	https://chrome.google.com/webstore/detail/google-input-tools/mclkkofklkfljcocdinagocijmpgbhab
	same as the one from translate.google.com