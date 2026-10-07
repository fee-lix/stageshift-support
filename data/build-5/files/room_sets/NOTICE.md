# Component-download scope — Build 5

This download contains the eleven retained audio responses and nine associated openly licensed or public-domain-source image adaptations. The independently generated Elveden and Sir Jack Lyons backgrounds are not distributed here. The app catalogue is retained as an audio/set reference; its background paths describe the app, and the download manifest marks these two images as omitted. The nine included image-generation records preserve the original prompts and credits.

The original app notice below is retained as an attribution/change reference. Its app-wide image count and facts-only research paragraphs describe the app and do not add files or grant rights to omitted project assets in this download.

---

# Room Set audio and image credits

StageShift — selected distribution catalogue (11 named rooms).

This notice accompanies only the audio, backgrounds and provenance included in this package. The existing generic-room collection retains its separate notices. Reusing a venue in several sets does not create another measurement or image.

Five unresolved audio sources and their associated images/provenance are excluded from this package. This selection is not a new license clearance or production approval for the retained content. No venue owner, measurement author or photographer has endorsed this app.

## Changes to the supplied materials

**Audio:** StageShift selected the documented measurement/channels below,
then used the native shared Plan-v1 authoring path to align the response,
remove its measured DC offset, resample where necessary to 48 kHz, apply the
recorded base gain once, and export stereo Float32 WAV. No other room's
measurement was substituted. The R1 response additionally has a ten-second
limit and a 100 ms terminal fade. The other 10 preparation records report
no duration-limit cut or terminal fade. A stereo container containing duplicated
mono is identified as such below; it is not a binaural measurement.

Each venue links to its bundled `provenance/<id>.json`, containing the selected
input SHA-256, final WAV SHA-256, decoder mapping, authoring tool/version,
sample counts, exact alignment, gain and fade decisions. These records describe
the actual new exports, not the earlier generic presets' render recipes.
See also the [native authoring workflow](../../docs/presets/authoring_workflow.md).

**Images:** all 11 backgrounds are AI-generated artistic reconstructions
made for StageShift with the built-in ImageGen tool. 9 used the
identified licensed/public-domain photographic input; Elveden and Sir Jack
Lyons used factual descriptions only. They are not documentary
photographs, exact architectural surveys, or depictions of the microphone
position. Changes include portrait recomposition, warm subdued lighting,
desaturated colour, dark lower areas for the app controls, and removal of
temporary equipment or people where specified. Source-specific changes are
listed below. Generated images were converted to JPEG. The bundled
[image generation record](image_generation.json) contains all 11 prompts,
output filenames and final SHA-256 hashes.

Photo credits and licenses apply independently from audio credits. The
Maeshowe and R1 image adaptations retain their stated ShareAlike terms below,
separately from the app's software license. References marked “facts only” were
not supplied as image-model input and no photograph license is claimed for them.
Source materials retain their applicable license warranty disclaimers.

## IEM CUBE

Assets: `ir/iem_cube.wav`, `images/iem_cube.jpg`.

**Audio credit:** Kaspar Müller, IEM / University of Music and Performing Arts
Graz (KUG), CUBE Soundfield measurements. The
[KUG dataset record](https://phaidra.kug.ac.at/detail/o:104435) uses
[Public Domain Mark 1.0](https://creativecommons.org/publicdomain/mark/1.0/),
which is preserved as that marking, not relabelled CC0. The embedded SOFA
description “Open Access” is not substituted for the record's marking.
[Original archive](https://phaidra.kug.ac.at/api/object/o:104435/download).
Selection: `cube_soundfield.sofa`, zero-based `Data.IR[16,0,0,:]`, central
receiver `(0,0,1.4)` m and emitter 0. The first/omnidirectional component is
duplicated to both channels; the unresolved directional ordering is not decoded.
The publisher had already band-pass filtered and shortened the source to 0.6 s.
[Processing and hashes](provenance/iem_cube.json).

**Image credit:** Franz Zotter, CUBE photograph in Jens Ahrens,
*Introduction to Ambisonics, Part 1: The Part With No Math*,
[arXiv:2512.07570v1, Figure 5 right](https://arxiv.org/html/2512.07570v1),
[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
[Exact photographic input](https://arxiv.org/html/2512.07570v1/pics/CUBE_Center_brightened.jpg).
AI reconstruction corrects panoramic projection into a rectangular view,
changes lighting/framing and omits temporary equipment. The source's existing
brightening, identified by its filename, is retained in the source reference.

## IEM Production Studio

Assets: `ir/iem_production_studio.wav`, `images/iem_production_studio.jpg`.

**Audio credit:** Markus Zaunschirm, IEM / KUG, IEM Production Studio KU100
measurements. [KUG record](https://phaidra.kug.ac.at/detail/o:76742),
[Public Domain Mark 1.0](https://creativecommons.org/publicdomain/mark/1.0/).
[Original WAV archive](https://phaidra.kug.ac.at/api/object/o:76742/comp/COMP000001)
and [measurement readme](https://phaidra.kug.ac.at/api/object/o:76742/comp/COMP000002).
Selection: `KU100Equalized_allRotations/Produktionsstudio_KU100_000Yaw_03_Center.wav`;
forward-facing KU100, centre speaker 03, original left/right ear channels.
The publisher's KU100 equalization is part of the source. Its approximately
0.341 s duration is preserved without inventing a longer studio response.
[Processing and hashes](provenance/iem_production_studio.json).

**Image credit:** Markus Zaunschirm, Matthias Frank and Franz Zotter (2020),
[Applied Sciences 10(5), 1631, Figure 1b](https://doi.org/10.3390/app10051631),
[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
[Exact PDF, page 3](https://mdpi-res.com/d_attachment/applsci/applsci-10-01631/article_deploy/applsci-10-01631.pdf).
Only the photographic panel was used, not the measurement diagram. No separate
photographer credit was supplied in the inspected figure. The AI reconstruction
interprets colour from the monochrome source, changes framing/light and removes
the measurement dummy head.

## Detmold Konzerthaus

Assets: `ir/detmold_konzerthaus.wav`, `images/detmold_konzerthaus.jpg`.

**Audio credit:** Sebastia Vicenc Amengual Gari, Banu Sahin, Dusty Eddy and
Malte Kob (2020), *Open Database of Spatial Room Impulse Responses at Detmold
University of Music*, [DOI 10.5281/zenodo.4116247](https://zenodo.org/records/4116247),
[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
[Original archive](https://zenodo.org/api/records/4116247/files/DetmoldSRIR_v01.zip/content),
member `SetC_DenseKH_LSOrchestra/Data/DummyHead/S3R163.wav`.
Selection: natural-acoustics loudspeaker-orchestra source S3 and main-floor
receiver R163, KU100, original two-channel order. No artificial reverberation
or WFS configuration was selected. The 1.5 s source is not lengthened.
Individual ear indices are not independently labelled in the inspected WAV;
its supplied KU100 channel order is preserved.
[Processing and hashes](provenance/detmold_konzerthaus.json).

**Image credit:** the same four dataset authors,
[MainDocumentation_v02.pdf, Figure 3.1 bottom-left photograph](https://zenodo.org/records/4116247/files/MainDocumentation_v02.pdf?download=1),
[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
No separate photographer credit was found. AI reconstruction changes framing
and lighting, preserving blue seating, dark walls and striped timber ceiling.

## Brahmssaal Detmold

Assets: `ir/detmold_brahmssaal.wav`, `images/detmold_brahmssaal.jpg`.

**Audio credit:** Sebastia Vicenc Amengual Gari, Banu Sahin, Dusty Eddy and
Malte Kob (2020), *Open Database of Spatial Room Impulse Responses at Detmold
University of Music*, [DOI 10.5281/zenodo.4116247](https://zenodo.org/records/4116247),
[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
[Original archive](https://zenodo.org/api/records/4116247/files/DetmoldSRIR_v01.zip/content),
member `SetA_SingleSources/Data/Brahmssaal/DummyHead/C1S1R4.wav`.
Selection: C1 without music stand, stage source S1, KU100 at R4, row 6,
seat 3 in the left aisle; natural acoustics, original two-channel order.
Individual ear indices are not independently labelled in the inspected WAV.
[Processing and hashes](provenance/detmold_brahmssaal.json).

**Image credit:** the same four dataset authors,
[MainDocumentation_v02.pdf, Figure 3.1 top-left photograph](https://zenodo.org/records/4116247/files/MainDocumentation_v02.pdf?download=1),
[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
No separate photographer credit was found. AI reconstruction removes the
microphone/cables, changes lighting/framing and retains the small hall's
curtained windows, circular lighting rails and chairs.

## Detmold Sommertheater

Assets: `ir/detmold_sommertheater.wav`, `images/detmold_sommertheater.jpg`.

**Audio credit:** Sebastia Vicenc Amengual Gari, Banu Sahin, Dusty Eddy and
Malte Kob (2020), *Open Database of Spatial Room Impulse Responses at Detmold
University of Music*, [DOI 10.5281/zenodo.4116247](https://zenodo.org/records/4116247),
[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
[Original archive](https://zenodo.org/api/records/4116247/files/DetmoldSRIR_v01.zip/content),
member `SetA_SingleSources/Data/SommerTheater/DummyHead/C1S1R3.wav`.
Selection: C1 without music stand, stage source S1, KU100 at R3, audience
row 6, seat 11; natural acoustics and original two-channel order. The source
documentation reports prior normalization to −6 dB per array while preserving
relative levels. Individual ear indices are not independently labelled in the
inspected WAV. [Processing and hashes](provenance/detmold_sommertheater.json).

**Image credit:** the same four dataset authors,
[MainDocumentation_v02.pdf, Figure 3.1 middle-left photograph](https://zenodo.org/records/4116247/files/MainDocumentation_v02.pdf?download=1),
[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
No separate photographer credit was found. AI reconstruction changes lighting
and framing, retaining the shallow side balconies, pale ceiling and dark seats.

## York Minster

Assets: `ir/york_minster.wav`, `images/york_minster.jpg`.

**Audio credit:** www.openairlib.net; Audiolab, University of York;
Damian T. Murphy. OpenAIR York Minster, `minster1_000_ortf_48k.wav`,
[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
[Original source page](https://www.openair.hosted.york.ac.uk/?page_id=797),
[exact WAV](https://webfiles.york.ac.uk/OPENAIR/IRs/york-minster/stereo/minster1_000_ortf_48k.wav).
Selection: original minster1 / 000 ORTF stereo capture, original channel order.
The original landing page was unavailable during the 2026 intake; the license
and credit are retained from the repository's previously pinned
[source notice](../church/license.txt), not claimed as a fresh page verification.
[Processing and hashes](provenance/york_minster.json).

**Image credit:** Mattana, *York York minster interior 014*, 6 June 2009,
[Wikimedia Commons source and PD-self dedication](https://commons.wikimedia.org/wiki/File:York_York_minster_interior_014.JPG),
including the file page's fallback grant; not relabelled CC0.
[Exact photographic input](https://upload.wikimedia.org/wikipedia/commons/3/38/York_York_minster_interior_014.JPG).
AI reconstruction recomposes the architectural detail into a portrait interior
and changes light/colour. The source is an upward view and does not establish
the full floor plan or measurement position.

## Maeshowe

Assets: `ir/maeshowe.wav`, `images/maeshowe.jpg`.

**Audio credit:** www.openairlib.net; Audiolab, University of York;
Damian T. Murphy. OpenAIR Maes Howe, `mh3_000_ortf_48k.wav`,
[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
[Original source page](https://www.openair.hosted.york.ac.uk/?page_id=602),
[exact WAV](https://webfiles.york.ac.uk/OPENAIR/IRs/maes-howe/stereo/mh3_000_ortf_48k.wav).
Selection: original mh3 / 000 ORTF stereo capture of the chamber, original
channel order. The source landing page was unavailable; credit/license are
retained from the pinned [source notice](../practice_room/license.txt).
[Processing and hashes](provenance/maeshowe.json).

**Image credit:** Richard Webb, *Maes Howe, interior*, 12 May 2002,
[Geograph photograph 4307137](https://www.geograph.org.uk/photo/4307137), via
[Wikimedia Commons](https://commons.wikimedia.org/wiki/File:Maes_Howe,_interior_-_geograph.org.uk_-_4307137.jpg),
[CC BY-SA 2.0](https://creativecommons.org/licenses/by-sa/2.0/).
AI reconstruction changes light, colour and portrait framing while following
the visible stone courses, slabs and side-chamber opening. The resulting
`images/maeshowe.jpg` adaptation is supplied under **CC BY-SA 2.0**, including
any rights in StageShift's adaptation contributions. This applies to this
image asset, independently of software code and the separately licensed audio;
retain attribution and the modification notice when reusing it.

## Elveden Marble Hall

Assets: `ir/elveden_marble_hall.wav`, `images/elveden_marble_hall.jpg`.

**Audio credit:** Matt Rogalsky, OpenAIR Elveden Hall Marble Hall stereo
response, [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
[Original source page](https://www.openair.hosted.york.ac.uk/?page_id=459),
[exact WAV `1a_marble_hall.wav`](https://webfiles.york.ac.uk/OPENAIR/IRs/elveden-hall-suffolk-england/stereo/1a_marble_hall.wav).
Selection: the original stereo pair of the specific Marble Hall, original
channel order, resampled from 44.1 kHz. The source landing page was unavailable;
credit/license are retained from the pinned
[source notice](../ceremonial_hall/license.txt).
[Processing and hashes](provenance/elveden_marble_hall.json).

**Image research credit — facts only:**
[Historic England, Elveden Hall, list entry 1037611](https://historicengland.org.uk/listing/the-list/list-entry/1037611/),
and [HeritageX, Elveden Hall](https://www.heritagexplore.com/houses/elveden-hall/).
The AI background was independently composed from factual descriptions of the
four-storey Carrara-marble atrium, cusped arches, recessed galleries and top-lit
dome. No reference photograph was supplied to ImageGen. No photographer name
or open adaptation license was established for the inspected HeritageX image;
none is invented or granted by this notice.

## Stockholm R1 Reactor Hall

Assets: `ir/stockholm_r1.wav`, `images/stockholm_r1.jpg`.

**Audio credit:** www.openairlib.net; Damian T. Murphy, OpenAIR R1 Nuclear
Reactor Hall ORTF capture, [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
[Original source page](https://www.openair.hosted.york.ac.uk/?page_id=626),
[exact WAV `r1_ortf-48k.wav`](https://webfiles.york.ac.uk/OPENAIR/IRs/r1-nuclear-reactor-hall/stereo/r1_ortf-48k.wav).
Selection: original ORTF stereo pair, original channel order. The approximately
20.28 s original was aligned, limited to ten seconds, and faded over the final
100 ms. This named-room export does not promote the separately blocked legacy
Small Hall preset. The source landing page was unavailable; credit/license are
retained from its pinned [source notice](../small_hall/license.txt), supported
by York's [acoustics teaching page](https://sites.google.com/york.ac.uk/music-technology-masterclass/home/1-acoustics).
[Processing and hashes](provenance/stockholm_r1.json).

**Image credit:** Alexandar Vujadinovic, *2021 KTH R1, image 1*,
3 November 2021,
[Wikimedia Commons source](https://commons.wikimedia.org/wiki/File:2021_KTH_R1,_image_1.jpg),
[CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/).
AI reconstruction changes light/colour/framing and makes coordinate markings
subtle while retaining the upper industrial chamber and walkways. It does not
reintroduce the removed reactor. The resulting `images/stockholm_r1.jpg`
adaptation is supplied under **CC BY-SA 4.0**, including any rights in
StageShift's adaptation contributions. This applies to this image asset,
independently of software code and the separately licensed audio; retain
attribution and the modification notice when reusing it.

## Usina del Arte — Symphonic Auditorium

Assets: `ir/usina_symphonic.wav`, `images/usina_symphonic.jpg`.

**Audio credit:** www.untref.edu.ar — Universidad Nacional de Tres de Febrero
(UNTREF), OpenAIR Usina del Arte Symphony Hall, main S1 P5,
[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
[Original source page](https://www.openair.hosted.york.ac.uk/?page_id=770),
[exact WAV `usina_main_s1_p5.wav`](https://webfiles.york.ac.uk/OPENAIR/IRs/usina-del-arte-symphony-hall/stereo/usina_main_s1_p5.wav).
Selection: source S1, position P5, original stereo pair/channel order from the
main symphonic auditorium. The source landing page was unavailable;
credit/license are retained from the pinned
[source notice](../concert_hall/license.txt).
[Processing and hashes](provenance/usina_symphonic.json).

**Image credit:** Gobierno de la Ciudad de Buenos Aires,
*Auditorio Usina de las Artes*, 23 May 2012,
[Wikimedia Commons / original Flickr provenance](https://commons.wikimedia.org/wiki/File:Auditorio_Usina_de_las_Artes.jpg),
[CC BY 2.0](https://creativecommons.org/licenses/by/2.0/).
AI reconstruction changes light/colour/framing and omits people and temporary
microphone stands, retaining the symphonic auditorium's timber, balconies,
brickwork, roof trusses and suspended panels.

## Sir Jack Lyons Concert Hall

Assets: `ir/jack_lyons.wav`, `images/jack_lyons.jpg`.

**Audio credit:** www.openairlib.net, OpenAIR Jack Lyons Concert Hall LP2,
[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
[Original source page](https://www.openair.hosted.york.ac.uk/?page_id=571),
[exact WAV `rir_jack_lyons_lp2_96k.wav`](https://webfiles.york.ac.uk/OPENAIR/IRs/jack-lyons-concert-hall-university-york/b-format/rir_jack_lyons_lp2_96k.wav).
Selection: LP2 four-channel first-order WXYZ FuMa capture at 96 kHz; explicitly
decoded by the shared W/X-centre, Y-side stereo mapping, then resampled to
48 kHz. This is a derived stereo rendering, not a recorded ear pair. The source
landing page was unavailable; credit/license are retained from the pinned
[source notice](../grand_concert_hall/license.txt).
[Processing and hashes](provenance/jack_lyons.json).

**Image research credit — facts only:** University of York,
[campus information](https://www.york.ac.uk/about/campus/) and
[self-guided campus tour](https://www.york.ac.uk/admin/hr/new-starters/welcome-to-york/on-campus/about/self-guided-tour-campus.pdf).
The inspected authentic interior photograph is credited by its source filename
to [Alex Holland, February 2021](https://www.york.ac.uk/media/abouttheuniversity/campus/UoY_Department%20of%20Music%20-%20Sir%20Jack%20Lyons%20Concert%20Hall_February%202021%20-%20Alex%20Holland-4.jpg).
The generated background was independently composed from descriptions of the
hexagonal hall, timber platform/slats, organ pipes, red seating and roof
trusses. No photograph was supplied to ImageGen and no open photo license is
claimed for Alex Holland's work.

## Evidence record

Source credits, license versions and modifications above are preserved from the documented source intake. Original source materials retain their license warranty disclaimers. The distribution inventory records the exact selected IDs and policy hash. Successful packaging does not establish permission beyond the stated source terms or close the separate platform, physical-device and production reviews.

