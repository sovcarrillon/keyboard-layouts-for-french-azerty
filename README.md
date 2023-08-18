keyboard layouts for Windows



better french azerty for math, physics and german
==================================================
** MODIFIED **
	capslock 
		does not lock non letters (same behavior as english US qwerty)
		gives access to caps letters with diacritic (majuscules accentuées)
** ADDED **
	acute accent "\´" dead key <span id="#acute-accent">§</span>
		altgr ^ (row below numbers next to letter P)
			touche avec déjà 2 diacritiques en dead key : ^ circonflexe et ¨ tréma diaeresis umlaut
		accent disponibles aussi sur certaines consonnes (pas seulement les voyelles)
			(ex : ẃ en welsh)
			ć, ń, ŕ, ś, ẃ, ź
			alternatives : d'autres existent et sont ajoutables
	math & logic & physics
		¬ "not operator" (also "not sign")
			altgr !
		≈ (~)
			altgr shift ~
			NOTE that we do not want to change ~ behavior as for example ~= has defined meaning in many programming languages and is very different from "approximately equal to"
		/ dead key
			altgr / 	suivi de
				inequalities
					= -> ≠
					< -> ≮
					> -> ≯
					TODO
						≃ -> ≄
						⩽ -> ≰
						⩾ -> ≱
						```
						2243	2244	// ≃ -> ≄
						2a7d	2270	// ⩽ -> ≰
						2a7e	2271	// ⩾ -> ≱
						```
				other
					o -> ø
					O -> Ø
						empty set
					h -> ℏ
						Planck constant
		∂ Partial Differential
			capslock shift d
		Newton's derivative notation https://en.wikipedia.org/wiki/Notation_for_differentiation#Newton's_notation
			˙ ẋ
				altgr numpad .
					then letter
				altgr shift ¨
					then letter
				supported letters:
					ȧ ḃ ċ ḋ ė ḟ ġ ḣ ṁ ṅ ȯ ṗ ṙ ṡ ṫ ẇ ẋ ẏ ż
				sadly UNSUPPORTED (not in unicode):
					greek letters
			use diaeresis ¨ for double derivative
				supported letters:
					ä ë ï ö ẗ ü ẅ ẍ ÿ
			UNSUPPORTED: more than 2 dots
		exposants et indices
			cf [indices et notes](#superscript-subscript)
		set symbols
			Ø empty set
			ø
				altgr / 	then 	O
				altgr / 	then 	o
			× cartesian product
				altgr *		(µ next to enter key, not on numpad)
		TODO other math stuff
			altgr with some key to enable math stuff : altgr numpad . or + or -   maybe ?
				(numpad require scan code and VK)
				≃
				⩽
				⩾
				congruent
				≃ (asymptotically equal to) ?
				sets
					N, Z, Q, R, C ?
					∈ "element of"
					∉ "not element of"
					⊂, ⊃ "subset of", "superset of"
					⊄, ⊅ "not subset of", "not superset of"
				...
		lettres grecques
			altgr lettre -> minuscule
				ou lorsque déjà utilisé (ex: €) 
					capslock shift lettre -> minuscule

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
				ε
					capslock shift e
						altgr e correspond déjà à €, hors on ne veux pas changer la disposition par défaut
				Ε 
					altgr shift e (normal)
			σ Σ ς sigma, final sigma	<span id="sigma">§</span>
				σ
					capslock shift s
						altgr s réservé pour le ß eszett allemand
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
	guillemets français 
		capslock <
		capslock shift < (ie. capslock >)
	·	"point médian"
		altgr .
		altgr shift .
	indices et notes <span id="superscript-subscript">§</span>
		via dead keys
		superscript
			shift ² 	ou  	capslock ²
				suivi des chiffres ⁰¹²³⁴⁵⁶⁷⁸⁹
				suivi des charactères ⁺⁻⁼⁽⁾
				suivi des lettres ᵃᵇᶜᵈᵉᶠᵍʰⁱʲᵏˡᵐⁿᵒᵖ𐞥ʳˢᵗᵘᵛʷˣʸᶻ(toutes sauf q)
				suivi des lettres grecques ᵝᵞᵟᵋᶿᶹᵠᶲᵡ
					MSKLC does not support U+107a5  (0071	107a5	// q -> 𐞥)
						TODO is there any workaround ?
				suivi de espace ˄ "Modifier Letter Up Arrowhead"
					(/!\ différent de ^ circonflexe notamment pour ne pas interférer avec l'existant : texte habituel, opérateur bit à bit XOR, bitwise XOR operator)
						alternative ⌄ "Up Arrowhead" ? no does not seem to work without modifier before
		subscript
			altgr ²
				suivi des chiffres ₀₁₂₃₄₅₆₇₈₉
				suivi des charactères ₊₋₌₍₎
				suivi des lettres ₐₑₕᵢⱼₖₗₘₙₒₚᵣₛₜᵤᵥₓ (uniquement aehijklmnoprstuvx, ie manque bcdfgqwyz)
				suivi des lettres grecques ᵦᵧᵨᵩᵪ
				suivi de espace ˅ "Modifier Letter Down Arrowhead"
					alternative ⌄ "Down Arrowhead" ? no does not seem to work without modifier before
	ligatures
		æ
			capslock shift a
		œ
			capslock shift o
		UNSUPPORTED capital ligatures
			Æ Œ
	allemand
		ß
			altgr s
		UNSUPPORTED
			capital ẞ (rarely used)
			„“ guillemets allemand
	espagnol
		¿
			altgr shift ?
		¡
			altgr shift ! 
	TODO various languages features
		dead key comme le azerty-afnor
			AltGr+Eu (AltGr+H) suivi d'une lettre
				to suuport unsupported stuff (ligatures, german, spanish, ...)

[#acute-accent]: #acute-accent
[#superscript-subscript]: #superscript-subscript

better french azerty for math, physics
=======================================
TODO same as former with no ß eszett on altgr s
	but instead 
		σ on: altgr s
		ς final sigma on: capslock shit s	(still also on: capslock shit c)
			```
			//σ Σ ς
			1f	S		SGCap	s	S	-1	03c3	03a3	// LATIN SMALL LETTER S, LATIN CAPITAL LETTER S, <none>, GREEK SMALL LETTER SIGMA, GREEK CAPITAL LETTER SIGMA
			-1	-1	0	S	03c2		// LATIN CAPITAL LETTER S, GREEK SMALL LETTER FINAL SIGMA
			//ß Σ σ
			1f	S		SGCap	s	S	-1	00df	03a3	// LATIN SMALL LETTER S, LATIN CAPITAL LETTER S, <none>, LATIN SMALL LETTER SHARP S (German), GREEK CAPITAL LETTER SIGMA
			-1	-1	0	S	03c3		// LATIN CAPITAL LETTER S, GREEK SMALL LETTER SIGMA
			```

greek azerty
=============
letters based on standard greek keyboard but mapped to french azerty instead of qwerty
	
** ADDED **
	supports improvements from [better french azerty for math, physics and german][] (added part only, as capslock behavior is made to follow qwerty keyboards)
		those improvements are totally transparent if you do not care
	altgr σ
		ς (final sigma)
	\` (accent grave) (altgr 7) combiné à une lettre grecque devient tonos
		reste un accent grave "backtick" lorsque suivi par une espace

** MODIFIED ** <span id="#greek-modified">§</span>
	decimal separator on numeric keypad
		. 	(instead of ,)
	^ (accent circomflexe à droite du P) totalement remplacé par dialytika tonos

** INFO **
	non letter keys are those displayed on french azerty except for @see [#greek-modified][]
	tonos produit par \` (accent grave) suivi d'une lettre
		altgr 7 *puis* lettre
	dialytika tonos produit par 
		^ (accent cironflexe à droite du P) *puis* lettre
			^ reste accessible via altgr 9
		shift w
			suit le clavier grec standard
	q
		q -> ;
		Q -> :
		suit le clavier grec standard

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
				fr-FR == 0000040c (see HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Keyboard Layout\DosKeybCodes )
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


uninstall keyboards
====================
Start  > Settings  > Apps > Apps & features 
	[keyboard name]
		More  > Uninstall

windows registry
==================
installed keyboards
	HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Keyboard Layouts

active, preloaded keyboards
	HKEY_USERS\.DEFAULT\Keyboard Layout\Preload
	HKEY_CURRENT_USER\Keyboard Layout\Preload
	HKEY_USERS\.DEFAULT\Control Panel\International\User Profile
	HKEY_USERS\.DEFAULT\Control Panel\International\User Profile System Backup

keyboard language codes
	HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Keyboard Layout\DosKeybCodes

@see also other interesting keyboards
=======================================
AFNOR
	[fr azerty AFNOR NF Z71-300] (https://www.boutique.afnor.org/fr-fr/norme/nf-z71300/interfaces-utilisateurs-dispositions-de-clavier-bureautique-francais/fa188960/1792) (/!\ norme payante, pas lue personnellement)
	description http://norme-azerty.fr/
	une implémentation Windows https://github.com/springcomp/optimized-azerty-win/tree/main
		doc de l'implémentation https://springcomp.github.io/optimized-azerty-win/
	une implémentation Linux https://github.com/Djyp/azerty_afnor

Korean
	IME with romaja support
		Nalgaeset Hangul Input System
		http://moogi.new21.org/en/ngs/index.htm
	some info about korean keyboards
		http://www.kbdedit.com/manual/low_level_special_nls_functions.html
		http://archives.miloush.net/michkap/archive/2012/04/30/10298801.html


chrome input tool extension
	https://chrome.google.com/webstore/detail/google-input-tools/mclkkofklkfljcocdinagocijmpgbhab
	same as the one from translate.google.com