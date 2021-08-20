# Observation Submission Template

This is an observation submission template to use when providing data to the AC CDC.

Jump to sections:
[Identifier](#identifier), [When](#when), [What](#what), [Who](#who), [Where](#where), [Observation details](#observation-details), [Collection data](#collection-data), [Notes](#notes)

Jump to fields: [`REFNUM`](#refnum), [`YYYY`](#yyyy), [`MM`](#mm), [`DD`](#dd), [`yyyy2`](#yyyy2), [`mm2`](#mm2), [`dd2`](#dd2), [`obDATEverbatim`](#obdateverbatim), [`SCNAME`](#scname), [`COMMON NAME`](#common-name), [`NAMETEMP`](#nametemp), [`NOTETAX`](#notetax), [`OBSERVER`](#observer), [`IDENTBY`](#identby), [`LATDEC`](#latdec), [`LONDEC`](#londec), [`LATDEC2`](#latdec2), [`LONDEC2`](#londec2),[`_NOTELOCcoordinates`](#noteloccoordinates),[`LOCUNCM`](#locuncm),[`_NOTELOClocuncm`](#noteloclocuncm) ,[`SURVEYSITE`](#surveysite) ,[`_NOTELOCsurveysite`](#notelocsurveysite) ,[`DIRECTIONS`](#directions) ,[`_NOTELOCdirections`](#notelocdirections) ,[`SITECODE`](#sitecode) ,[`ELEVmin`](#elevmin),[`OBEVID`](#obevid) ,[`OBABUN`](#obabun) ,[`OBABUNSITE`](#obabunsite) ,[`OBCOUNT`](#obcount) ,[`OBASSP`](#obassp) ,[`OBDESC`](#obdesc) ,[`OBACTIV`](#obactiv) ,[`OBPHEN`](#obphen) ,[`OBSEX`](#obsex) ,[`HABITAT`](#habitat) ,[`OBTHREAT`](#obthreat) ,[`ENVIRONMENTAL`](#environmental) ,[`URL`](#url) ,[`PROJECT`](#project) ,[`PROTOCOL`](#protocol),[`COLLECTION`](#collection) ,[`COLLNUM`](#collnum) ,[`COLLDUP`](#colldup) ,[`ACCNUM`](#accnum),[`NOTE1`](#note1) ,[`NOTE2`](#note2)

### Identifier
#### `REFNUM`
| |`REFNUM`|
| -------------  |-------------|
| **Definition** | Record ID (e.g., field or collection number) assigned by observer.|
| **Comments**   | If the field is used consistently by observers, it can be used to join, merge or relate records to existing records in our database. It can also be used by the observer to match data to personal datasets.      |
| **Examples**   | `TP1234`, `NS-RP025-2_617`, `Tupper-Barrens_525`|
| **Data type**   | TEXT |
| **Data validation restrictions**   | Each `REFNUM` value must be unique. |

### When
#### `YYYY`
| |    `YYYY`      |
| -------------  |-------------|
| **Definition** |Year of observation  |
| **Comments**   |    Can include ‘X’ characters for any digits that are uncertain. When the observation was made for multiple, known, years between these dates submit a record for each known year. |
| **Examples**   | `2021`, `199X`, `19XX` |
| **Data type**   | TEXT |
| **Data validation restrictions**   | **Allow:** Text length **Data:** equal to **Length:** 4 |

#### `MM`
| |     `MM`    |
| -------------  |-------------|
| **Definition** | Month of observation |
| **Comments**   | If missing use `XX`|
| **Examples**   | `12`, `XX`, `5` |
| **Data type**   | TEXT |
| **Data validation restrictions**   | **Allow:** Text length **Data:** between **Minimum:** 1 **Maximum:** 2 |

#### `DD`
|           |     `DD`     |
| -------------  |-------------|
| **Definition** | Day of observation |
| **Comments**   |If missing use `XX`|
| **Examples**   | `31`, `2`, `XX` |
| **Data type**   | TEXT |
| **Data validation restrictions**   | **Allow:** Text length **Data:** between **Minimum:** 1 **Maximum:** 2 |

#### `yyyy2`
|           |   `yyyy2`      |
| -------------  |-------------|
| **Definition** | End year of a date range for observation |
| **Comments**   | If your observation took place over a range of years, use this field for the end year. Use [`YYYY`](#yyyy) to record the start year of the range. |
| **Examples**   | `2021`, `199X`, `19XX` |
| **Data type**   | TEXT |
| **Data validation restrictions**   | **Allow:** Text length **Data:** equal to **Length:** 4 |

#### `mm2`
|           |    `mm2`     |
| -------------  |-------------|
| **Definition** | End month of a date range for observation |
| **Comments**   | If your observation took place over a range of months, use this field for the end month. Use [`MM`](#mm) to record the start month of the range.|
| **Examples**   | `12`, `5` |
| **Data type**   | TEXT |
| **Data validation restrictions**   | **Allow:** Text length **Data:** between **Minimum:** 1 **Maximum:** 2 |

#### `dd2`
|           |    `dd2`     |
| -------------  |-------------|
| **Definition** | End day of a date range for observation |
| **Comments**   |If your observation took place over a range of days, use this field for the end day. Use [`DD`](#dd) to record the start day of the range.|
| **Examples**   |`31`, `2` |
| **Data type**   | TEXT |
| **Data validation restrictions**   | **Allow:** Text length **Data:** between **Minimum:** 1 **Maximum:** 2 |

#### `obDATEverbatim`
|           |    `obDATEverbatim`     |
| -------------  |-------------|
| **Definition** | This field can hold any text description of the date or details about uncertainty |
| **Comments**   ||
| **Examples**   |`spring 2010`, `collected sometime between 4 June and 23 July` |
| **Data type**   | TEXT |
| **Data validation restrictions**   |  |

### What
#### `SCNAME`
|           |    `SCNAME`      |
| -------------  |-------------|
| **Definition** | Scientific name as given by reference |
| **Comments**   |       |
| **Examples**   | `Clemmys insculpta` |
| **Data type**   | TEXT |
| **Data validation restrictions**   | |

#### `COMMON NAME`
|           |     `COMMON NAME`     |
| -------------  |-------------|
| **Definition** | English name |
| **Comments**   |       |
| **Examples**   |`Wood Turtle` |
| **Data type**   | TEXT |
| **Data validation restrictions**   | |

#### `NAMETEMP`
|           |   `NAMETEMP`       |
| -------------  |-------------|
| **Definition** | Temporary name. Use this field to store names you are uncertain about and names not yet identified to the species level.  |
| **Comments**   |  Would include chemical tests used in lichen identification. If we make change to ID, details are included here. If changed by others (e.g., herbarium) could go in IDENTBY. |
| **Examples**   | |
| **Data type**   | TEXT |
| **Data validation restrictions**   |`Poa`,  `indet.`|

#### `NOTETAX`
|           |    `NOTETAX`      |
| -------------  |-------------|
| **Definition** | Relevant information on identification |
| **Comments**   |       |
| **Examples**   | `orig. ID C. subdentata (=C. spinigera)`, `Hypericum boreale/mutilum` |
| **Data type**   | TEXT |
| **Data validation restrictions**   | |

### Who
#### `OBSERVER`
|           | `OBSERVER`       |
| -------------  |-------------|
| **Definition** | Person who collected datum in field |
| **Comments**   | Use this format `lastname1, firstname1; lastname2, firstname2`. Use `unknown` only if the observer is confidently known to be unknown. Otherwise, use `blank`. If the first name or last name is missing, use a `?` to indicate a missing name. |
| **Examples**   | `Blaney, Sean; Robinson, Sarah; Mazerolle, David`, `Blaney, Sean; et al.`, `unknown`, `<blank>`, `Cochran, ?` `Atlasser ID: <number>`, `Blaney, Sean; Robinson, Sarah; Mazerolle, David, plus 8 observers`|
| **Data type**   | TEXT |
| **Data validation restrictions**   | |

#### `IDENTBY`
|           |    `IDENTBY`     |
| -------------  |-------------|
| **Definition** | Person identifying record (esp. where diff. from observer) |
| **Comments**   | If history of identification (e.g., changes over time), include this information here. Can contain dates and institution info. Format names as in [OBSERVER](#observer).|
| **Examples**   |`Blaney, Sean` |
| **Data type**   | TEXT |
| **Data validation restrictions**   | |

### Where
#### `LATDEC`
|           |    `LATDEC`      |
| -------------  |-------------|
| **Definition** | Latitude of observation in Decimal Degrees |
| **Comments**   |       |
| **Examples**   |`42.12345` |
| **Data type**   | DECIMAL NUMBER |
| **Data validation restrictions**   | **Allow:** Decimal **Data:** between **Minimum:** -90 **Maximum:** 90 |

#### `LONDEC`
|           |     LONDEC     |
| -------------  |-------------|
| **Definition** | Longitude of observation in Decimal Degrees |
| **Comments**   |       |
| **Examples**   |`-64.12345` |
| **Data type**   | DECIMAL NUMBER |
| **Data validation restrictions**   | **Allow:** Decimal **Data:** between **Minimum:** -180 **Maximum:** 180 |

#### `LATDEC2`
|           |     `LATDEC2`     |
| -------------  |-------------|
| **Definition** | If observation is a linear transect, add end point here |
| **Comments**   |       |
| **Examples**   |`42.12345` |
| **Data type**   | DECIMAL NUMBER |
| **Data validation restrictions**   | **Allow:** Decimal **Data:** between **Minimum:** -90 **Maximum:** 90 |

#### `LONDEC2`
|           |     `LONDEC2`   |
| -------------  |-------------|
| **Definition** | If observation is a linear transect, add end point here |
| **Comments**   |       |
| **Examples**   |`-64.12345` |
| **Data type**   | DECIMAL NUMBER |
| **Data validation restrictions**   | **Allow:** Decimal **Data:** between **Minimum:** -180 **Maximum:** 180 |

#### `_NOTELOCcoordinates`
|           |   `_NOTELOCcoordinates`       |
| -------------  |-------------|
| **Definition** | Basis of coordinates and/or remark upon extent |
| **Comments**   |       |
| **Examples**   | `geolocation from GPS`|
| **Data type**   | TEXT |
| **Data validation restrictions**   | |

#### `LOCUNCM`
|           |     `LOCUNCM`     |
| -------------  |-------------|
| **Definition** |Estimated horizontal uncertainty distance of location (metres)  |
| **Comments**   |Use '10' for GPS locations|
| **Examples**   | `10`, `50`, `500`, `1000` |
| **Data type**   | POSITIVE INTEGER |
| **Data validation restrictions**   | **Allow:** Whole number **Data:** greater than or equal to **Minimum:** 10 |

#### `_NOTELOClocuncm`
|           |     `_NOTELOClocuncm`     |
| -------------  |-------------|
| **Definition** | Further information on location uncertainty  |
| **Comments**   |       |
| **Examples**   | |
| **Data type**   | TEXT |
| **Data validation restrictions**   | |

#### `SURVEYSITE`
|           |     `SURVEYSITE`     |
| -------------  |-------------|
| **Definition** | Major landmark: permanent town or land feature nearby. Single placename of general locality, especially designated or proposed Protected Area. |
| **Comments**   |    No abbreviations. `SURVEYSITE` must be a placename. |
| **Examples**   | `Saint John River` |
| **Data type**   | TEXT |
| **Data validation restrictions**   | |

#### `_NOTELOCsurveysite`
|           |    `_NOTELOCsurveysite`      |
| -------------  |-------------|
| **Definition** | Further information about survey site.  |
| **Comments**   |       |
| **Examples**   | |
| **Data type**   | TEXT |
| **Data validation restrictions**   | |

#### `DIRECTIONS`
|           |     `DIRECTIONS`     |
| -------------  |-------------|
| **Definition** | Detailed instructions for re-finding observation. Distance and direction from a landmark |
| **Comments**   |       |
| **Examples**   | `S of Gagetown, 100m upstream from mouth of Mud Creek` |
| **Data type**   | TEXT |
| **Data validation restrictions**   | |

#### `_NOTELOCdirections`
|           |   `_NOTELOCdirections`       |
| -------------  |-------------|
| **Definition** | Further information about directions  |
| **Comments**   |       |
| **Examples**   | |
| **Data type**   | TEXT |
| **Data validation restrictions**   | |

#### `SITECODE`
|           |    `SITECODE`      |
| -------------  |-------------|
| **Definition** | Site reference code specific to the project or data collection event |
| **Comments**   |   Helps link observation back to data provider's study sites    |
| **Examples**   | |
| **Data type**   | TEXT |
| **Data validation restrictions**   | |

#### `ELEVmin`
|           |    `ELEVmin`      |
| -------------  |-------------|
| **Definition** |Elevation in metres  |
| **Comments**   |    Should be integer between 0 and 820 if in Maritimes   |
| **Examples**   |`70`, `152`, `30`, `9` |
| **Data type**   | POSITIVE INTEGER |
| **Data validation restrictions**   | **Allow:** Whole number **Data:** greater than or equal to **Minimum:** 0 |

### Observation details
#### `OBEVID`
|           |    `OBEVID`      |
| -------------  |-------------|
| **Definition** | Nature of the evidence associated with the observation  |
| **Comments**   |  Default is ‘sight record’     |
| **Examples**   | See **Data validation restrictions**  
| **Data type**   | LOWERCASE TEXT |
| **Data validation restrictions**   | Allowable values are: `sight record`, `specimen`,`photo`,`specimen;photo`,`aural detection`,`sound recording`,`video recording`,`indirect (e.g., scat, pellets, tracks, browse)`,`perennial nest site`,`iNaturalist`|

#### `OBABUN`
|           |    `OBABUN `   |
| -------------  |-------------|
| **Definition** | Verbal description of frequency with reference to the abundance at a specific point location |
| **Comments**   |       |
| **Examples**   | See **Data validation restrictions**  
| **Data type**   | LOWERCASE TEXT |
| **Data validation restrictions**   | Allowable values are: `abundant`,`locally common`,`scattered`,`rare`|

#### `OBABUNSITE`
|           |    `OBABUNSITE`      |
| -------------  |-------------|
| **Definition** | Verbal description of frequency with reference to the larger survey area |
| **Comments**   |       |
| **Examples**   | See **Data validation restrictions**  
| **Data type**   | LOWERCASE TEXT |
| **Data validation restrictions**   | Allowable values are: `common within survey site`,`rare within survey site`,`uncommon within survey site`|

#### `OBCOUNT`
|           |   `OBCOUNT`      |
| -------------  |-------------|
| **Definition** | The number of individuals/units (e.g,. The number of adults, young, eggs) |
| **Comments**   |   Use special characters like ~, +, < only when absolutely necessary.    |
| **Examples**   | `10-50`, `1`, `>100` |
| **Data type**   | POSITIVE INTEGER, sometimes TEXT |
| **Data validation restrictions**   ||

#### `OBASSP`
|           |   `OBASSP`       |
| -------------  |-------------|
| **Definition** | Associated Species; species observed with taxon recorded |
| **Comments**   |   Use scientific names; separate species by semicolon. Include host or nectaring plant species here if available; can also add to [`HABITAT`](#habitat) if deemed appropriate |
| **Examples**   | `Abies balsamea; Picea rubens; Acer rubrum; Betula allegheniensis; Betula papyrifera; Onoclea sensibilis; Matteuccia struthiopteris`, `Leucodon brachypus`, `Thuja occidentalis; Betula papyrifera; Picea glauca`, `Nectaring on Malus pumila` |
| **Data type**   | TEXT |
| **Data validation restrictions**   ||

#### `OBDESC`
|           |     `OBDESC`     |
| -------------  |-------------|
| **Definition** | Description of state, condition or appearance of individual/group |
| **Comments**   |   E.g., patch dimensions, number of clumps, interesting markings or state of individual, e.g. 'pregnant'. Behavior and activity go in [`OBACTIV`](#obactiv)    |
| **Examples**   | `corticolous`, `collected incidentally with CJC 4129`, `only 1 or 2 populations oberved`|
| **Data type**   | TEXT |
| **Data validation restrictions**   ||

#### `OBACTIV`
|           |  `OBACTIV`        |
| -------------  |-------------|
| **Definition** | Activity or behavior observed |
| **Comments**   |  For birds use formal MBBA breeding evidence statements found in file      |
| **Examples**   | `just molted`, `Confirmed breeding: Adult carrying food. 5 adults hunting and bringing food back to nest sites`, `terrestrial, stationary, in sun`, `Nesting`, `mating` |
| **Data type**   | TEXT |
| **Data validation restrictions**   ||

#### `OBPHEN`
|           |   `OBPHEN`       |
| -------------  |-------------|
| **Definition** | Phenology (bud, flower, seed; age or life stage) |
| **Comments**   |  Full names: adult, juvenile, immature     |
| **Examples**   | `adult`, `mature`, `flowering`, `fruiting`, `senescent` |
| **Data type**   | LOWERCASE TEXT |
| **Data validation restrictions**   | Lowercase text only |

#### `OBSEX`
|           |    `OBSEX`      |
| -------------  |-------------|
| **Definition** | Gender of taxon |
| **Comments**   |  Full words: male; female; 1 male, 2 females    |
| **Examples**   | `female`, `male`, `1 male, 1 female`|
| **Data type**   | LOWERCASE TEXT |
| **Data validation restrictions**   | Lowercase text only |

#### `HABITAT`
|           |    `HABITAT`     |
| -------------  |-------------|
| **Definition** | Habitat in which the taxon was found |
| **Comments**   |       |
| **Examples**   |`gravel island in river` |
| **Data type**   | TEXT |
| **Data validation restrictions**   | |

#### `OBTHREAT`
|           |    `OBTHREAT`     |
| -------------  |-------------|
| **Definition** | Information about natural or anthropogenic threats to the identified taxon at the place it was observed |
| **Comments**   |       |
| **Examples**   |`numerous ATV tracks through nesting area`, `tree harvesting edge of swamp`, `vegetation control under powerline` |
| **Data type**   | TEXT |
| **Data validation restrictions**   | |

#### `ENVIRONMENTAL`
|           |   `ENVIRONMENTAL`      |
| -------------  |-------------|
| **Definition** | A general field for any environmental conditions it is deemed valuable to retain |
| **Comments**   |  Cloud cover, temperature, wind     |
| **Examples**   | `temp: 23C; cloud cover: partial`|
| **Data type**   | TEXT |
| **Data validation restrictions**   | |

#### `URL`
|           |    `URL`      |
| -------------  |-------------|
| **Definition** | URL of associated record for iNat, eBird checklist if applicable.  |
| **Comments**   |  For the record, not for a photo associated with the record     |
| **Examples**   | |
| **Data type**   | TEXT |
| **Data validation restrictions**   | |

#### `PROJECT`
|           |    `PROJECT`      |
| -------------  |-------------|
| **Definition** | Name for project for which the data were collected.  |
| **Comments**   |   Helpful for sorting collections of data in our database   |
| **Examples**   | |
| **Data type**   | TEXT |
| **Data validation restrictions**   | |

#### `PROTOCOL`
|           |    `PROTOCOL`      |
| -------------  |-------------|
| **Definition** | Type of survey used for data collection |
| **Comments**   |   This provides an indication of biases and level of search effort    |
| **Examples**   | See **Data validation restrictions**  
| **Data type**   | LOWERCASE TEXT |
| **Data validation restrictions**   | Allowable values are: `incidental`,`point count`,`area search`,`trapping`,`songmeter`,`eBird - Incidental`,`eBird - Travelling`|

### Collection data
#### `COLLECTION`
|           |   `COLLECTION`       |
| -------------  |-------------|
| **Definition** |Museum or institution holding specimen  |
| **Comments**   | Abbreviated as: {ACAD, MICH, NBM…}       |
| **Examples**   |`NFM`, `ACAD, NSPM` `UNB`|
| **Data type**   | TEXT |
| **Data validation restrictions**   | |

#### `COLLNUM`
|           |   `COLLNUM`       |
| -------------  |-------------|
| **Definition** | Field or collection number assigned by the observer |
| **Comments**   |       |
| **Examples**   |`TP1234`, `3907`, `6365322-22-NOWA` |
| **Data type**   | TEXT |
| **Data validation restrictions**   | |

#### `COLLDUP`
|           |     `COLLDUP`     |
| -------------  |-------------|
| **Definition** | Number of duplicates of the specimen |
| **Comments**   |       |
| **Examples**   | `1`, `2`|
| **Data type**   | POSITIVE INTEGER |
| **Data validation restrictions**   |  **Allow:** Whole number **Data:** greater than **Minimum:** 0|

#### `ACCNUM`
|           |   `ACCNUM`       |
| -------------  |-------------|
| **Definition** | Museum Accession number (assigned by museum/institution) |
| **Comments**   |       |
| **Examples**   |`NBM-00484`, `B144361`, `OBS504457741` |
| **Data type**   | TEXT |
| **Data validation restrictions**   | |


### Notes
#### `NOTE1`
|           |    `NOTE1`      |
| -------------  |-------------|
| **Definition** | Miscellaneous information of value that cannot be entered in other fields |
| **Comments**   |  Ensure these do not contain values that fit in other standard fields    |
| **Examples**   | |
| **Data type**   | TEXT |
| **Data validation restrictions**   | |

#### `NOTE2`
|           |    `NOTE2`      |
| -------------  |-------------|
| **Definition** | Miscellaneous information of value that cannot be entered in other fields |
| **Comments**   |   Ensure these do not contain values that fit in other standard fields      |
| **Examples**   | |
| **Data type**   | TEXT |
| **Data validation restrictions**   | |

