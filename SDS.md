# 🧭 System Description Specification (SDS)

## Númer teymis og höfundar
Hópur 3, Björgvin Þeyr Guðmundsson og Konráð Jóel Jónasson.

## Heiti kerfis
Kerfisskrá

## Hvað er kerfið?
Kerfisskráin heldur utan um upplýsingar um starfsmenn og sýnir hvernig þeir tengjast í fyrirtækinu. Þetta er ætlað fyrir mannauðsdeild eða starfsfólk hennar.

## Tilgangur
Kerfisskráin á að auðvelda starfsfólki að finna upplýsingar og stjórnendur í fyrirtækinu og halda skipulagi uppfærðu.

## Afmörkun (Scope)
**Innan scope:** 
Helstu atriði sem kerfið á að styðja:
- Skrá og vista upplýsingar um starfsmenn.
- Skoða og uppfæra upplýsingar starfsmanna.
- Stjórna starfstitlum og deildatengingum.
- Leita að starfsmönnum eftir nafni, deild eða starfstitli.
- Birta skipulagstré fyrirtækisins með yfirmönnum og undirmönnum.
- Leyfa stjórnendum og HR starfsfólki að framkvæma breytingar samkvæmt aðgangsheimildum.
**Utan scope:** 
Atriði sem kerfið nær ekki yfir:
- Launakerfi og launavinnsla.
- Ráðningarferli og umsóknastjórnun.
- Frammistöðumat starfsmanna.
- Tímaskráning og viðverukerfi.
- Orlofs- og veikindaskráningar.
- Samþætting við bókhaldskerfi.

## Samhengi kerfis (context) 
Kerfið starfar innan fyrirtækis og er notað til að halda utan um upplýsingar um starfsmenn, deildir og stjórnskipulag. Helstu notendur kerfisins eru almennir starfsmenn, stjórnendur og mannauðsdeild. Kerfið hefur einnig samskipti við auðkenningarkerfi fyrirtækisins t.d Micorsoft authenticator og AD sem sér um innskráningu og aðgangsstýringar.

            Innskráningarkerfi
                     |
                     |
                     v
Starfsmenn  <--> Kerfisskráin <--> Mannauður
                     ^
                     |
                     |
                Stjórnendur

- **Fólk og hagsmunaaðilar:** Helstu notendur kerfisins eru almennir starfsmenn, stjórnendur og mannauðsdeild. Kerfisstjórar sem hafa umsjón með aðgangsstýringum og rekstri kerfisins.
- **Ytri kerfi og þjónustur:** Micorsoft authenticator og AD. 
- **Önnur atriði í umhverfinu:** Reglur fyrirtækisins um aðgangsstýringar og persónuvernd. Skipurit fyrirtækisins og stjórnskipulag.
- **Mörk kerfisins:** 
**Tilheyrir kerfinu:**
- Geymsla og birting starfsmannaupplýsinga.
- Síuvirkni fyrir starfsmenn.
- Birting skipurits fyrirtækisins.
- Umsýsla starfstitla, deilda og tengsla milli starfsmanna.
- Aðgangsstýringar innan kerfisins út frá hlutverkum.
**Tilheyrir samhengi kerfisins:**
- Active Directory og Microsoft Authenticator.
- Reglur fyrirtækisins og persónuverndarkröfur.

## Tenging við SRS
- Sjá nánari kröfuskipan í [SRS](SRS/SRS.md) (viðskiptakröfur, fídusar, notendakröfur o.s.frv.).
