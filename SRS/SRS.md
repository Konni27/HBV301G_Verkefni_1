# 📄 Software Requirements Specification (SRS)

## 1. Inngangur
### 1.1 Tilgangur
Kerfið heldur utan um upplýsingar um starfsmenn og sýnir hvernig þeir tengjast í fyrirtækinu. Það á að auðvelda starfsfólki að finna upplýsingar og stjórnendum að halda skipulagi uppfærðu.

### 1.2 Umfang og mörk kerfisins

Kerfið nær yfir skráningu og uppfærslu starfsmannaupplýsinga, leit að starfsmönnum og birtingu skipulagstrés. Það nær ekki yfir laun, tímaskráningu eða önnur mannauðskerfi. Notendur nota kerfið í vafra og gögn eru vistuð í bakenda eða gagnagrunni.

### 1.3 Skilgreiningar
| Hugtak | Skýring |
|--------|---------|
| SRS | Software Requirements Specification |
| HR | Mannauðsdeild eða starfsfólk hennar |
| Skipulagstré | Yfirlit yfir starfsmenn, deildir og stjórnendur |


### 1.4 Tilvísanir
- ISO/IEC/IEEE International Standard - Systems and software engineering -- Life cycle processes -- Requirements engineering," in ISO/IEC/IEEE 29148:2018(E) , vol., no., pp.1-104, 30 Nov. 2018, doi: 10.1109/IEEESTD.2018.8559686.ISO/IEC/IEEE 29

---

## 2. Almenn lýsing
### 2.1 Notendahópar
- **HR starfsfólk:** Leitar að og uppfærir upplýsingar um starfsmenn.
- **Stjórnendur:** Skoða starfsmenn í sínum deildum og bæta fólki við deildir.
- **Almennir starfsmenn:** Skoða skipulagstréð og leita að samstarfsfólki.

### 2.2 Viðskiptaávinningur
- Kerfið safnar upplýsingum um starfsmenn á einn stað og gerir þær auðveldari að finna. Það gefur einnig betri yfirsýn yfir deildir og stjórnendur.

---

## 3. Kröfur fyrir kerfið

### 3.1 Viðskiptakröfur
| ID                                        | Titill                    |
|-------------------------------------------|---------------------------|
| [BREQ-1](business_requirements.md#breq-1) | Upplýsingar um starfsmenn |
| [BREQ-2](business_requirements.md#breq-2) | Einföld flokkun fyrir fyrirtæki |

### 3.2 Kerfiskrafa
| ID                              | Titill                 |
|---------------------------------|------------------------|
| [SR-1](system_requirement.md#sr-1) | Flokkun og vistun gagna |

### 3.3 Eiginleikar (Features)
| ID                     | Titill                 |
|------------------------|------------------------|
| [F-1](feature.md#f-1)  | Starfsmannaupplýsingar |
| [F-2](feature.md#f-2)  | Skipulagstré |
| [F-3](feature.md#f-3)  | Leit og síun |

### 3.4 Notendakröfur
| ID                                   | Titill                  | Eiginleiki |
|--------------------------------------|-------------------------|------------|
| [UR-1](user_requirement.md#ur-1)     | HR finnur upplýsingar um starfsmann | F-1        |
| [UR-2](user_requirement.md#ur-2)     | Stjórnandi bætir fólki við deild | F-1        |
| [UR-3](user_requirement.md#ur-3)     | Starfsmaður sér sitt skipulagstré | F-2        |
| [UR-4](user_requirement.md#ur-4)     | HR uppfærir upplýsingar | F-1        |
| [UR-5](user_requirement.md#ur-5)     | Stjórnandi skoðar undirmenn | F-2        |
| [UR-6](user_requirement.md#ur-6)     | Starfsmaður finnur samstarfsfólk | F-3        |

### 3.5 Virknikröfur
| ID                                          | Titill                                      | Notendakrafa |
|---------------------------------------------|---------------------------------------------|--------------|
| [FR-1](functional_requirement.md#fr-1)      | Leit að starfsmanni | UR-1         |
| [FR-2](functional_requirement.md#fr-2)      | Birting upplýsinga | UR-1         |
| [FR-3](functional_requirement.md#fr-3)      | Leitarniðurstöður | UR-1         |
| [FR-4](functional_requirement.md#fr-4)      | Val á starfsmanni og deild | UR-2         |
| [FR-5](functional_requirement.md#fr-5)      | Starfsmaður bættur við deild | UR-2         |
| [FR-6](functional_requirement.md#fr-6)      | Vistun deildar | UR-2         |
| [FR-7](functional_requirement.md#fr-7)      | Auðkenning notanda | UR-3         |
| [FR-8](functional_requirement.md#fr-8)      | Sjálfvirkt skipulagstré | UR-3         |
| [FR-9](functional_requirement.md#fr-9)      | Birting samstarfsmanna | UR-3         |
| [FR-10](functional_requirement.md#fr-10)    | Breyting upplýsinga | UR-4         |
| [FR-11](functional_requirement.md#fr-11)    | Uppfærsla starfstitils | UR-4         |
| [FR-12](functional_requirement.md#fr-12)    | Vistun breytinga | UR-4         |
| [FR-13](functional_requirement.md#fr-13)    | Birting skipulagstrés | UR-5         |
| [FR-14](functional_requirement.md#fr-14)    | Birting starfsmanna deildar | UR-5         |
| [FR-15](functional_requirement.md#fr-15)    | Birting stöðu stjórnanda | UR-5         |
| [FR-16](functional_requirement.md#fr-16)    | Leit að starfsmanni | UR-6         |
| [FR-17](functional_requirement.md#fr-17)    | Síun eftir deild | UR-6         |
| [FR-18](functional_requirement.md#fr-18)    | Birting tengiliðaupplýsinga | UR-6         |

### 3.6 Viðskiptareglur
| ID                                  | Titill                     |
|-------------------------------------|----------------------------|
| [BRG-1](business_rule.md#brg-1)     | Aðgangur eftir stöðu |
| [BRG-2](business_rule.md#brg-2)     | Einn beinn yfirmaður |

### 3.7 Gæðaeiginleikar
| ID                                      | Titill                     |
|-----------------------------------------|----------------------------|
| [QA-1](quality_attribute.md#qa-1)       | Auðveld stjórnun |
| [QA-2](quality_attribute.md#qa-2)       | Auðveld notkun |

### 3.8 Takmarkanir
| ID                              | Titill                |
|---------------------------------|-----------------------|
| [C-1](constraint.md#c-1)        | Innskráning og MFA |
| [C-2](constraint.md#c-2)        | Vefkerfi án uppsetningar |

### 3.9 Ytri skil (Interfaces)
| ID                                      | Titill                |
|-----------------------------------------|-----------------------|
| [UI-1](external_interface.md#ui-1)      | Tengingar við bakenda |
| [UI-2](external_interface.md#ui-2)      | Notendaviðmót |

---

## 4. Viðaukar
### 4.1 Orðalisti
- Helstu hugtök eru útskýrð hér að neðan.

  | Hugtak | Skilgreining |
  |--------|--------------|
  | Deild | Hópur starfsmanna innan fyrirtækisins |
  | MFA | Fjölþátta auðkenning |

### 4.2 Samþykktir
- Kennari: ____________________  
- Nemandi: ____________________
