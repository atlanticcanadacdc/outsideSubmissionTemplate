# Observation Submission Template

This is an observation submission template to use when submitting data to the AC CDC.

Jump to sections:
[Identifier](#identifier), [When](#when), [What](#what), [Who](#who), [Where](#where), [Observation details](#observation-details), [Collection data](#collection-data), [Source of data](#source-of-data), [Notes](#notes)

Jump to fields: [REFNUM](#refnum), [`YYYY`](#-yyyy-), [`MM`](#-mm-), [`DD`](#-dd-), [`yyyy2`](#-yyyy2-), [`mm2`](#-mm2-), [`dd2`](#-dd2-), [`obDATEverbatim`](#-obdateverbatim-), [`SCNAME`](#-scname-), [`COMMON NAME`](#-common-name-), [`NAMETEMP`](#-nametemp-), [`NOTETAX`](#-notetax-), [`OBSERVER`](#-observer-), [`IDENTBY`](#-identby-), [Where](#where), [`LATDEC`](#-latdec-), [`LONDEC`](#-londec-)

### Identifier
#### `REFNUM`
| |`REFNUM`|
| -------------  |-------------|
| **Definition** | Record ID (e.g., field or collection number) assigned by observer.|
| **Comments**   | If the field is used consistently by observers, it can be used to join, merge or relate records to existing records in our database. It can also be used by the observer to match data to their personal datasets.      |
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
| **Comments**   | If your observation took place over a range of years, use this field for the end year. Use [`YYYY`](#-yyyy-) to record the start year of the range. |
| **Examples**   | `2021`, `199X`, `19XX` |
| **Data type**   | TEXT |
| **Data validation restrictions**   | **Allow:** Text length **Data:** equal to **Length:** 4 |

#### `mm2`
|           |    `mm2`     |
| -------------  |-------------|
| **Definition** | End month of a date range for observation |
| **Comments**   | If your observation took place over a range of months, use this field for the end month. Use [`MM`](#-mm-) to record the start month of the range.|
| **Examples**   | `12`, `5` |
| **Data type**   | TEXT |
| **Data validation restrictions**   | **Allow:** Text length **Data:** between **Minimum:** 1 **Maximum:** 2 |

#### `dd2`
|           |    `dd2`     |
| -------------  |-------------|
| **Definition** | End day of a date range for observation |
| **Comments**   |If your observation took place over a range of days, use this field for the end day. Use [`DD`](#-dd-) to record the start day of the range.|
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

|           |     SURVEYSITE     |
| -------------  |-------------|
| **Definition** |  |
| **Comments**   |       |
| **Examples**   | |

|           |    `_NOTELOCsurveysite`      |
| -------------  |-------------|
| **Definition** |  |
| **Comments**   |       |
| **Examples**   | |

|           |     DIRECTIONS     |
| -------------  |-------------|
| **Definition** |  |
| **Comments**   |       |
| **Examples**   | |

|           |   `_NOTELOCdirections`       |
| -------------  |-------------|
| **Definition** |  |
| **Comments**   |       |
| **Examples**   | |

|           |    SITECODE      |
| -------------  |-------------|
| **Definition** |  |
| **Comments**   |       |
| **Examples**   | |

|           |    ELEVmin      |
| -------------  |-------------|
| **Definition** |  |
| **Comments**   |       |
| **Examples**   | |

### Observation details

|           |    OBEVID      |
| -------------  |-------------|
| **Definition** |  |
| **Comments**   |       |
| **Examples**   | |

|           |    OBABUN      |
| -------------  |-------------|
| **Definition** |  |
| **Comments**   |       |
| **Examples**   | |


|           |    OBABUNSITE      |
| -------------  |-------------|
| **Definition** |  |
| **Comments**   |       |
| **Examples**   | |

|           |   OBCOUNT       |
| -------------  |-------------|
| **Definition** |  |
| **Comments**   |       |
| **Examples**   | |

|           |   OBASSP       |
| -------------  |-------------|
| **Definition** |  |
| **Comments**   |       |
| **Examples**   | |

|           |     OBDESC     |
| -------------  |-------------|
| **Definition** |  |
| **Comments**   |       |
| **Examples**   | |

|           |  OBACTIV        |
| -------------  |-------------|
| **Definition** |  |
| **Comments**   |       |
| **Examples**   | |

|           |   OBPHEN       |
| -------------  |-------------|
| **Definition** |  |
| **Comments**   |       |
| **Examples**   | |

|           |    OBSEX      |
| -------------  |-------------|
| **Definition** |  |
| **Comments**   |       |
| **Examples**   | |

|           |    HABITAT      |
| -------------  |-------------|
| **Definition** |  |
| **Comments**   |       |
| **Examples**   | |


|           |    OBTHREAT      |
| -------------  |-------------|
| **Definition** |  |
| **Comments**   |       |
| **Examples**   | |

|           |   ENVIRONMENTAL       |
| -------------  |-------------|
| **Definition** |  |
| **Comments**   |       |
| **Examples**   | |

|           |    URL      |
| -------------  |-------------|
| **Definition** |  |
| **Comments**   |       |
| **Examples**   | |

|           |    PROJECT      |
| -------------  |-------------|
| **Definition** |  |
| **Comments**   |       |
| **Examples**   | |

|           |    PROTOCOL      |
| -------------  |-------------|
| **Definition** |  |
| **Comments**   |       |
| **Examples**   | |

### Collection data

|           |   COLLECTION       |
| -------------  |-------------|
| **Definition** |  |
| **Comments**   |       |
| **Examples**   | |

|           |   COLLNUM       |
| -------------  |-------------|
| **Definition** |  |
| **Comments**   |       |
| **Examples**   | |

|           |     COLLDUP     |
| -------------  |-------------|
| **Definition** |  |
| **Comments**   |       |
| **Examples**   | |

|           |   ACCNUM       |
| -------------  |-------------|
| **Definition** |  |
| **Comments**   |       |
| **Examples**   | |

### Source of data

|           |   BESTSOURCE       |
| -------------  |-------------|
| **Definition** |  |
| **Comments**   |       |
| **Examples**   | |

### Notes

|           |    NOTE1      |
| -------------  |-------------|
| **Definition** |  |
| **Comments**   |       |
| **Examples**   | |

|           |    NOTE2      |
| -------------  |-------------|
| **Definition** |  |
| **Comments**   |       |
| **Examples**   | |

