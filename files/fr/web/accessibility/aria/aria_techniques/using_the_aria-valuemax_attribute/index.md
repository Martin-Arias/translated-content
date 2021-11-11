---
title: Utiliser l'attribut aria-valuemax
slug: Web/Accessibility/ARIA/ARIA_Techniques/Using_the_aria-valuemax_attribute
tags:
  - ARIA
  - Accessibilité
  - Attribut
translation_of: Web/Accessibility/ARIA/ARIA_Techniques/Using_the_aria-valuemax_attribute
original_slug: Accessibilité/ARIA/Techniques_ARIA/Utiliser_l_attribut_aria-valuemax
---
<h3 id="Description">Description</h3>

<p>Cette technique présente l’utilisation de l’attribut <a href="http://www.w3.org/TR/wai-aria/states_and_properties#aria-valuemax">aria-valuemax</a>.</p>

<p>L’attribut <code>aria-valuemax</code> est utilisé pour définir la valeur maximale autorisée pour un composant à intervalle tels qu’une barre de progression <code>progressbar</code>, un bouton rotatif <code>spinbutton</code> ou un curseur <code>slider</code>. Si <a href="/fr/Accessibilité/ARIA/Techniques_ARIA/Utiliser_l_attribut_aria-valuenow"><code>aria-valuenow</code></a> a des valeurs minimale et maximale connues, le développeur devrait fournir les propriétés de <code>aria-valuemax</code> et <a href="/fr/Accessibilité/ARIA/Techniques_ARIA/Utiliser_l_attribut_aria-valuemin"><code>aria-valuemin</code></a>. La valeur de <code>aria-valuemax</code> <strong>DOIT</strong> être supérieure ou égale à celle de <a href="/fr/Accessibilité/ARIA/Techniques_ARIA/Utiliser_l_attribut_aria-valuemin"><code>aria-valuemin</code></a>.</p>

<p><code>aria-valuemax</code> est un attribut <strong>obligatoire</strong> des rôles <a href="/fr/Accessibilité/ARIA/Techniques_ARIA/Utiliser_le_rôle_slider">slider</a>, <a href="/fr/Accessibilité/ARIA/Techniques_ARIA/Utiliser_le_rôle_scrollbar">scrollbar</a> et <a href="/fr/Accessibilité/ARIA/Techniques_ARIA/Utiliser_le_rôle_spinbutton">spinbutton</a>.</p>

<h3 id="Valeurs">Valeurs</h3>

<p>Représentation d’un nombre par une chaîne</p>

<h3 id="Effets_possibles_sur_les_agents_utilisateurs_et_les_technologies_d’assistance">Effets possibles sur les agents utilisateurs et les technologies d’assistance</h3>

<p>Si la valeur <code>aria-valuemax</code> n’est pas déterminée, ou si <code>aria-valuemin</code> n’est pas inférieure ou égale à la valeur de <code>aria-valuemax</code>, cela créera une condition d’erreur qui sera gérée par la technologie d’assistance.</p>

<div class="note"><p><strong>Note :</strong> il existe plusieurs points de vue sur la façon dont les technologies d’assistance devraient traiter cette technique. L’information fournie ci-dessus est l’une de ces opinions et n’est pas normative.</p></div>

<h3 id="Exemples">Exemples</h3>

<h4 id="Exemple_1">Exemple 1:</h4>

<p>L’extrait de code ci-dessous montre un curseur basique avec une valeur maximale de 10.</p>

<pre class="brush: html">&lt;div role="slider" aria-valuenow="4" aria-valuemin="1" aria-valuemax="10"&gt;
</pre>

<h3 id="Notes">Notes</h3>

<h3 id="Utilisés_avec_les_rôles_ARIA">Utilisés avec les rôles ARIA</h3>

<ul>
 <li><a href="/fr/Accessibilité/ARIA/Techniques_ARIA/Utiliser_le_rôle_progressbar">progressbar</a> ;</li>
 <li><a href="/fr/Accessibilité/ARIA/Techniques_ARIA/Utiliser_le_rôle_scrollbar">scrollbar</a> ;</li>
 <li><a href="/fr/Accessibilité/ARIA/Techniques_ARIA/Utiliser_le_rôle_slider">slider</a> ;</li>
 <li><a href="/fr/Accessibilité/ARIA/Techniques_ARIA/Utiliser_le_rôle_spinbutton">spinbutton</a>.</li>
</ul>

<h3 id="Techniques_ARIA_connexes">Techniques ARIA connexes</h3>

<ul>
 <li><a href="/fr/Accessibilité/ARIA/Techniques_ARIA/Utiliser_l_attribut_aria-valuemin">aria-valuemin</a> ;</li>
 <li><a href="/fr/Accessibilité/ARIA/Techniques_ARIA/Utiliser_l_attribut_aria-valuenow">aria-valuenow</a> ;</li>
 <li><a href="/fr/Accessibilité/ARIA/Techniques_ARIA/Utiliser_l_attribut_aria-valuetext">aria-valuetext</a>.</li>
</ul>

<h3 id="Autres_ressources">Autres ressources</h3>

<ul>
 <li><a href="http://www.w3.org/TR/wai-aria/states_and_properties#aria-valuemax">Spécification WAI-ARIA pour l’attribut <code>aria-valuemax</code></a>.</li>
</ul>