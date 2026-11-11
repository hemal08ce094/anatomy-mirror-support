# Attribution

These meshes are adapted from **Z-Anatomy - The libre 3D atlas of anatomy**
(<https://github.com/Z-Anatomy/Models-of-human-anatomy>, commit `dd53423db366c3b881a402c2b3061783b98d6322`),
licensed under CC BY-SA 4.0, which is itself built on **BodyParts3D**, © The Database Center for
Life Science (<https://dbarchive.biosciencedbc.jp/en/bodyparts3d/>). Z-Anatomy credits BodyParts3D
under CC BY-SA 2.1 Japan; the BodyParts3D site now offers it under CC BY 4.0. Some cranial nerve
geometry in Z-Anatomy is adapted from "Cranial Nerves and Foramina", University of Dundee, CAHID,
CC BY 4.0.

Credit lines as the upstream asks for them:

- "Z-Anatomy - The libre 3D atlas of anatomy - CC-BY-SA 4.0"
- "BodyParts3D - The Database Center for Life Science - CC-BY-SA 2.1 Japan"

This folder is shared under CC BY-SA 4.0 (see `LICENSE`).

## What was changed

- Exported from Z-Anatomy's `Startup.blend` with Blender 5.2.3 LTS; curves (nerves, vessels)
  evaluated to tube meshes with their bevel; mirrored objects re-wound so normals face outward.
- Registered to the AnatomyMirror head frame: a uniform-scale similarity fitted on the skull
  (scale 1.02619, skull RMS 1.86 mm after fit), then centimetres, origin between
  the eyeball centres, +x subject's left, +y up, +z forward, Frankfurt plane level.
- Soft tissue that broke through the AnatomyMirror skin (BodyParts3D 4.0) was pulled just under it:
  vertices outside the skin or closer than 0.8 mm to it (1.8 mm for the temporalis, 2 mm for the
  masseter) were moved along the skin normal to that depth.
- Cut flat at the neck where the structure continues below the head; left and right copies and
  sub-parts merged into one file per structure; welded, decimated to a triangle budget, smooth
  normals recomputed.

## Files

| file | structure | Z-Anatomy objects |
|---|---|---|
| `meshes/muscles__platysma.obj` | Platysma | Platysma |
| `meshes/muscles__frontalis.obj` | Frontalis | Frontalis muscle |
| `meshes/muscles__occipitalis.obj` | Occipitalis | Occipitalis muscle |
| `meshes/muscles__epicranial_aponeurosis.obj` | Epicranial aponeurosis | Epicranial aponeurosis |
| `meshes/muscles__orbicularis_oculi.obj` | Orbicularis oculi | Orbital part of orbicularis oculi, Palpebral part of orbicularis oculi |
| `meshes/muscles__corrugator_supercilii.obj` | Corrugator supercilii | Corrugator supercilii |
| `meshes/muscles__procerus.obj` | Procerus | Procerus muscle |
| `meshes/muscles__nasalis.obj` | Nasalis | Nasalis muscle |
| `meshes/muscles__depressor_septi_nasi.obj` | Depressor septi nasi | Depressor septi nasi |
| `meshes/muscles__levator_labii_superioris_alaeque_nasi.obj` | Levator labii superioris alaeque nasi | Levator nasolabialis |
| `meshes/muscles__levator_labii_superioris.obj` | Levator labii superioris | Levator labii superioris |
| `meshes/muscles__levator_anguli_oris.obj` | Levator anguli oris | Levator anguli oris |
| `meshes/muscles__zygomaticus_major.obj` | Zygomaticus major | Zygomaticus major muscle |
| `meshes/muscles__zygomaticus_minor.obj` | Zygomaticus minor | Zygomaticus minor muscle |
| `meshes/muscles__risorius.obj` | Risorius | Risorius muscle |
| `meshes/muscles__buccinator.obj` | Buccinator | Bucinator |
| `meshes/muscles__orbicularis_oris.obj` | Orbicularis oris | Orbicularis oris muscle |
| `meshes/muscles__depressor_anguli_oris.obj` | Depressor anguli oris | Depressor anguli oris |
| `meshes/muscles__depressor_labii_inferioris.obj` | Depressor labii inferioris | Depressor labii inferioris |
| `meshes/muscles__mentalis.obj` | Mentalis | Mentalis muscle |
| `meshes/muscles__masseter.obj` | Masseter | Deep part of masseter, Superficial part of masseter |
| `meshes/muscles__temporalis.obj` | Temporalis | Temporalis muscle |
| `meshes/muscles__lateral_pterygoid.obj` | Lateral pterygoid | Inferior head of lateral pterygoid muscle, Superior head of lateral pterygoid muscle |
| `meshes/muscles__medial_pterygoid.obj` | Medial pterygoid | Medial pterygoid muscle |
| `meshes/vessels__cerebral_arterial_circle.obj` | Cerebral arterial circle | Anterior communicating artery, Posterior communicating artery |
| `meshes/vessels__common_carotid_artery.obj` | Common carotid artery | Left common carotid artery, Right common carotid artery |
| `meshes/vessels__external_carotid_artery.obj` | External carotid artery | Ascending pharyngeal artery, External carotid artery |
| `meshes/vessels__facial_artery.obj` | Facial artery | Angular artery, Facial artery, Inferior labial artery, Submental artery, Superior labial artery |
| `meshes/vessels__superficial_temporal_artery.obj` | Superficial temporal artery | Frontal branch of superficial temporal artery, Superficial temporal artery, Transverse facial artery |
| `meshes/vessels__occipital_artery.obj` | Occipital artery | Occipital artery |
| `meshes/vessels__maxillary_artery.obj` | Maxillary artery | Accessory branch of middle meningeal artery, Anterior deep temporal artery, Artery of pterygoid canal, Buccal artery, Descending palatine artery, Greater palatine artery, Inferior alveolar artery, Infra-orbital artery, Maxillary artery, Mental branch of inferior alveolar artery, Middle meningeal artery, Mylohyoid branch of inferior alveolar artery, Posterior deep temporal artery, Posterior lateral nasal branches of sphenopalatine artery., Posterior septal branches of sphenopalatine artery, Posterior superior alveolar artery |
| `meshes/vessels__ophthalmic_artery.obj` | Ophthalmic artery | Anterior ethmoidal artery, Anterior septal branches of anterior ethmoidal artery, Central retinal artery, Lacrimal artery, Long posterior ciliary arteries, Ophthalmic artery, Posterior ethmoidal artery, Septal branches of posterior ethmoidal artery, Short posterior ciliary arteries, Supra-orbital artery, Supratrochlear artery |
| `meshes/vessels__internal_carotid_artery.obj` | Internal carotid artery | Internal carotid artery |
| `meshes/vessels__vertebral_artery.obj` | Vertebral artery | Anterior spinal artery, Vertebral artery |
| `meshes/vessels__basilar_artery.obj` | Basilar artery | Basilar artery, Lateral pontine branches of basilar artery, Medial pontine branches of basilar artery |
| `meshes/vessels__cerebellar_arteries.obj` | Cerebellar arteries | Anterior inferior cerebellar artery, Posterior inferior cerebellar artery, Superior cerebellar artery |
| `meshes/vessels__anterior_cerebral_artery.obj` | Anterior cerebral artery | Anterior cerebral artery, Callosomarginal artery, Frontal branches of callosomarginal artery, Orbitofrontal branches of anterior cerebral artery, Pericallosal artery |
| `meshes/vessels__posterior_cerebral_artery.obj` | Posterior cerebral artery | Lateral occipital artery, Medial occipital artery, Parieto-occipital artery, Posterior cerebral artery |
| `meshes/vessels__middle_cerebral_artery.obj` | Middle cerebral artery | Artery of central sulcus, Artery of precentral sulcus, Deep cervical artery, Insular branches of middle cerebral artery (M2), Insular branches of middle cerebral artery (M2-segment), Lateral frontobasal artery, Middle cerebral artery (M1-segment), Middle cerebral artery (M3 segment), Middle cerebral artery (M3-segment), Parietal branches of middle cerebral artery, Postcentral arterial branch, Posterior parietal artery, Prefrontal artery, Temporal branches of middle cerebral artery, Transverse cervical artery |
| `meshes/veins__dural_venous_sinuses.obj` | Dural venous sinuses | Anterior intercavernous sinus, Basilar venous plexus, Cavernous sinus, Inferior petrosal sinus, Inferior sagittal sinus, Occipital sinus, Posterior intercavernous sinus, Sigmoid sinus, Straight sinus, Superior petrosal sinus, Superior sagittal sinus, Transverse sinus |
| `meshes/veins__internal_jugular_vein.obj` | Internal jugular vein | Internal jugular vein |
| `meshes/veins__external_jugular_vein.obj` | External jugular vein | External jugular vein, Occipital vein, Posterior auricular vein |
| `meshes/veins__facial_vein.obj` | Facial vein | Angular vein, Common facial vein, Facial vein, Inferior labial veins, Submental vein, Superior labial vein |
| `meshes/veins__retromandibular_vein.obj` | Retromandibular vein | Anterior division of retromandibular vein, Maxillary veins, Posterior division of retromandibular vein, Retromandibular vein, Superficial temporal veins |
| `meshes/veins__ophthalmic_veins.obj` | Ophthalmic veins | Inferior ophthalmic vein, Superior ophthalmic vein |
| `meshes/veins__other_neck_veins.obj` | Veins of the neck | Lingual vein, Superior thyroid vein, Vertebral vein |
| `meshes/nerves__facial_nerve.obj` | Facial nerve (VII) | Facial nerve (VII) |
| `meshes/nerves__chorda_tympani.obj` | Chorda tympani | Chorda tympani |
| `meshes/nerves__trigeminal_nerve.obj` | Trigeminal nerve (V) | Motor root of trigeminal nerve, Sensory root of trigeminal nerve, Trigeminal nerve (V) |
| `meshes/nerves__ophthalmic_nerve.obj` | Ophthalmic nerve | Ophthalmic nerve |
| `meshes/nerves__maxillary_nerve.obj` | Maxillary nerve | Maxillary nerve, Meningeal branch of maxillary nerve |
| `meshes/nerves__mandibular_nerve.obj` | Mandibular nerve | Anterior division of mandibular nerve, Buccal nerve, Posterior division of mandibular nerve |
| `meshes/nerves__inferior_alveolar_nerve.obj` | Inferior alveolar nerve | Inferior alveolar nerve, Mental nerve, Nerve to mylohyoid muscle |
| `meshes/nerves__lingual_nerve.obj` | Lingual nerve | Lingual nerve |
| `meshes/nerves__optic_nerve.obj` | Optic nerve (II) | Optic nerve (II) |
| `meshes/nerves__olfactory_nerve.obj` | Olfactory nerve (I) | Olfactory nerve (I) |
| `meshes/nerves__oculomotor_nerve.obj` | Oculomotor nerve (III) | Oculomotor nerve (III) |
| `meshes/nerves__trochlear_nerve.obj` | Trochlear nerve (IV) | Trochlear nerve (IV) |
| `meshes/nerves__abducens_nerve.obj` | Abducens nerve (VI) | Abducens nerve (VI) |
| `meshes/nerves__glossopharyngeal_nerve.obj` | Glossopharyngeal nerve (IX) | Glossopharyngeal nerve (IX) |
| `meshes/nerves__vagus_nerve.obj` | Vagus nerve (X) | Vagus nerve (X) |
| `meshes/nerves__accessory_nerve.obj` | Accessory nerve (XI) | Accessory nerve (XI) |
| `meshes/nerves__hypoglossal_nerve.obj` | Hypoglossal nerve (XII) | Hypoglossal nerve (XII) |
| `meshes/glands__parotid_gland.obj` | Parotid gland | (Accessory parotid gland), Parotid duct, Parotid gland |
| `meshes/glands__submandibular_gland.obj` | Submandibular gland | Submandibular duct, Submandibular gland |
| `meshes/glands__sublingual_gland.obj` | Sublingual gland | Sublingual gland |
| `meshes/glands__lacrimal_gland.obj` | Lacrimal gland | Lacrimal gland |
| `meshes/cartilage__nasal_cartilages.obj` | Nasal cartilages | Lateral process of nasal septal cartilage, Major alar cartilage, Nasal septal cartilage |
| `meshes/cartilage__laryngeal_cartilages.obj` | Laryngeal cartilages | Arytenoid cartilage, Corniculate cartilage, Cricoid cartilage, Epiglottis, Thyroid cartilage |
| `meshes/eyeAdnexa__tarsal_plates.obj` | Tarsal plates | Inferior tarsus, Superior tarsus |
| `meshes/eyeAdnexa__lacrimal_drainage.obj` | Lacrimal sac and duct | Lacrimal canaliculus, Lacrimal sac, Nasolacrimal duct |
