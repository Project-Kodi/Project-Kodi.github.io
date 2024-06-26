
> [!NOTE]
> Support us on Patreon: <a href="https://patreon.com/ProjectKodi">patreon.com/ProjectKodi</a>

# Project Kodi - The Sports Database Pyhton
## metadata.thesportsdb.python

<p align="left">
<ul>
    <li>File naming tools for Sports Database: <a href="https://www.tinymediamanager.org/">TinyMediaManager</a> | <a href="https://gitlab.com/tinyMediaManager">TinyMediaManager - Gitlab</a> (and yet not supported: Media Companion, MediaElch, Radarr, Sonarr, Jellyfin,.. help and contact the software manufacturers!)</li>
    <li>Kodi Forum: The Sports Database Pyhton - (metadata.thesportsdb.python): <a href="https://forum.kodi.tv/showthread.php?tid=368208">TheSportsDB Python Scraper (for Nexus and Later)</a></li>
    <li>Download: Use the Project Kodi Repository in Kodi: <a href="https://project-kodi.github.io/">https://project-kodi.github.io/</a></li>
    <li>Download Example Files: <a href="https://raw.githubusercontent.com/Project-Kodi/Project-Kodi.github.io/main/Information/The%20Sports%20Database%20Python%20-%20metadata.thesportsdb.python/File%20Naming%20%26%20Tools/Example%20files%20for%20naming/Example%20files%20for%20naming.zip">Example files for naming.zip</a></li>
  </ul>
  </p>

Github Source: <a href="https://github.com/Project-Kodi/Project-Kodi.github.io/tree/main/Information/The%20Sports%20Database%20Python%20-%20metadata.thesportsdb.python">https://github.com/Project-Kodi/Project-Kodi.github.io/tree/main/Information/The%20Sports%20Database%20Python%20-%20metadata.thesportsdb.python</a>
  
  


# Documentation

- Addon Download and Installation

- Addon Settings

- Addong Using

## Addon Download and Installation


### 1. Install - Project-Kodi Repository


<p align="left">
	<ul>
		<li>Go to the Kodi file manager.</li>
		<li>Click on "Add source".</li>
		<li>The path for the source is: <code>https://Project-Kodi.github.io/</code> (Give it the name "Project Kodi Repository").</li>
		<li>Go to "Addons".</li>
		<li>In addons, install an addon from zip.  When it asks for the location, select "Project Kodi Repository", and install <a href="repository.project.kodi-1.0.1.zip">repository.project.kodi-1.0.1.zip</a>.</li>
		<li>Now the repository is available in Kodi.</li>
		<li>Additionally, you should turn on automatic updating: Go to “Addons”, select “User Addons”, then “Addon Repository”, select “Project Kodi Repository” and activate automatic updating.</li>
	</ul>
</p>

### 2. Install - The Sports Database Addon

<p align="left">
	<ul>
		<li>Go to "Addons", select "Install from repository".</li>
		<li>Select the "Project Kodi Repository".</li>
		<li>Go to Information provider, tv information and choose The Sports Database Python</li>
	</ul>
</p>

<img height="600" src="_images/addon01.jpg" alt="Addon Settings">

## Addon Settings

### Addon Settings - General 

- Language

  - **Preferred language (Fallback EN)**: Title/description and other texts are retrieved in this selected language. If the desired language is not available, English will be used.

- Trailer

  - **Enable Trailer**: Is for episodes only, information is already stored in Kodi, but trailers are not yet supported for episodes.

  - **Addon Player**: Used for playing the trailer (not used at this time)

- API:

  - **TSDB - API Version**: Here you can switch between the API versions. You only get the latest features with version 2.

  - **Sleep in seconds each API call**: Since only 100 requests are allowed per minute, you need at least 0.1 seconds delay. (Fast server/workstations)

<img height="600" src="_images/addon02.jpg" alt="Addon Settings">

### Addon Settings - NFO

- Scraper

  - **Ignore local NFO file**: With Kodi you can't turn off the search for NFO files, but you can bypass it. The NFO file must contain at least one of the following tags with data. Example `<tsdb>4234</tsdb>` or `<episodeguide>{tsdb:4234}</episodeguide>`. Tags: `<title> <showtitle> <originaltitle> <strLeague> <tsdb> <episodeguide> <tvshowsource>`.

> [!TIP]
> Before scraping the first time, you should remove any existing NFO files without TSDB Data in your Sports Series folder.
> After the first run, Kodi then always fetches the most current data from the Internet, even if an NFO file with TSDB Data has been saved with the scraper.

- NFO

  - **Write NFO file**: First, the scraper imports all information into the database and then writes a desired NFO file according to guidelines. `https://kodi.wiki/view/NFO_files/TV_shows`

  - **Overwrite NFO files if exists**: If an NFO file exists, it will be overwritten

  - **Save in the respective TVShow/Season/Episode folder**: The NFO file is stored in the series folder. Example: `C:\Sport-Series\Formula 1\tvshow.nfo`

    - **Choose own path - TVShow**: You can choose any path regardless of the operating system.

    - **Choose own path - Season**: You can choose any path regardless of the operating system.
    
    - **Choose own path - Episode**: You can choose any path regardless of the operating system.

  - **NFO filename TVShow**: You can change the name of the NFO file. Option 1: `tvshow.nfo` 2: `tvshowname.nfo` | It is stored in the series folder or in the desired path.

  - **NFO filename Season**: You can change the name of the NFO file. Option 1: `seasonXX.nfo` - stored in tvshow folder Option 2: `season.nfo` - stored in the tvshow/seasonXX folder. Both options also work in the desired path.

  - **NFO filename Episode**: You can change the name of the NFO file. At this time only one option here. Option 1: `episodename.nfo` | is stored in the Series/Season X/ folder or in the desired path.

<img height="600" src="_images/addon03.jpg" alt="Addon Settings">

<img height="600" src="_images/addon04.jpg" alt="Addon Settings">


### Addon Settings - Modifications 

- Title

  - **Add Date to episode name**: A date is added to the title of the episode in Kodi. Example - normal: `04. Venezuela vs Mexico` | Example changed:  `04. Venezuela vs Mexico - Sat 3rd Mrz`

  - **Exclude Leagues by name**: If you want to add the feature, but not to all TV shows/leagues, then you can exclude leagues with names here. Example: `Formula 1, Copa America, French Ligue 1` (I) 

> [!TIP]
> Even if you have problems viewing the series in the menu if you have activated the function, you should add this TVShow/League to the list. (Example: no numbers are displayed next to the episodes or the series is not recognized at all)

<img height="600" src="_images/addon05.jpg" alt="Addon Settings">




### Addon Settings - Artwork 

- TVShows

  - **Download Poster in TVShow folder**: Here you can switch on whether poster should also be saved locally in the series folder.

  - **Poster filename for TVShow**: You can control the file naming here. In the series folder as `poster.jpg` or as `seriesname-poster.jpg`.

  - **Download Fanart in TVShow folder**: Here you can switch on whether fanart should also be saved locally in the series folder. (At this time, only 1 fanart from max.5 possible - Update..)

  - **Fanart filname for TVShow**: You can control the file naming here. In the series folder as `fanart.jpg` or as `seriesname-fanart.jpg`.

  - **Download Banner in TVShow folder**: Here you can switch on whether banner should also be saved locally in the series folder.

  - **Banner filename TVShow**: You can control the file naming here. In the series folder as `banner.jpg` or as `seriesname-banner.jpg`.

  - **Download ClearLogo in TVShow folder**: Here you can switch on whether clearlogo should also be saved locally in the series folder.

  - **ClearLogo filename for TVShow**: You can control the file naming here. In the series folder as `clearlogo.jpg` or as `seriesname-clearlogo`.jpg.

  - <b>Feature DL Season Posters - open</b>


- Seasons

  - **Use League Poster for all Seasons**: There are currently not yet separate posters available for all seasons in the TSDB. If you activate the function, the addon will automatically take the league poster for all series.

> [!TIP] 
> If you deactivate the function, all available season posters will be used/downloaded. If none is available for a season, the TVShow/League poster will be used

- Character Art (Player)

  - **User Character Art**: If you activate this function, the desired character arts will be added to the Kodi database.

  - **Character Art Version**: There are 2 different representations of players/participants. From the front as `Player Cutout` and as a picture where the player/participant is in motion `Player Action Render`. 

  - **Download Character Art**: The character art is not only loaded into the Kodi database, it is also downloaded but a maximum of 10 images are saved in the desired folder.

  - **Character Art filename**: There are 2 options: 1. `characterart.png - characterart9.png` or 2. `tvshowfoldername-characterart.png - tvshowfoldername-characterart9.png`.

  - **Save in the respective TVShow folder**: If activated, the images will be stored in the series folder.

  - **Choose your own path**: You can also enter your own path for saving the images.


<img height="600" src="_images/addon06.jpg" alt="Addon Settings">


<img height="600" src="_images/addon07.jpg" alt="Addon Settings">


### Addon Settings - Logging & Other

- Logging

  - **Verbose debug logging**: Lots of details are written. In normal operation, this feature should be disabled. It slows down the scraper extremely.

  - **Verbose debug logging extreme**: Many more details are recorded. In normal operation, this feature should be disabled. It slows down the scraper extremely. 1 series can generate a log larger than 1 GB!

- Premium 

  - **API Key TheSportsDB**: If you are a supporter of TheSportsDB.com, you can enter your own API key. But this is not necessary as we have already integrated a key. In the later future, there could be features that only Patreon supporters can activate.

> [!IMPORTANT]
> **Support us on Patreon:** <a href="https://www.patreon.com/ProjectKodi">patreon.com/ProjectKodi</a>

- Support

  - **Visit us @ Github**: This is our Github Website: <a href="https://project-kodi.github.io/">Project-Kodi.github.io</a> | Our Kodi Repository and documentation: <a href="https://github.com/Project-Kodi/Project-Kodi.github.io/tree/main">github.com/Project-Kodi/Project-Kodi.github.io/</a> 

  - **Visit TheSportsDB Discord - Support**: You get support for the addon via Discord but also for the data from TheSportsDB.com A large active community. <a href="https://discord.gg/pFvgaXV">discord.gg/pFvgaXV</a>

<img height="600" src="_images/addon08.jpg" alt="Addon Settings">



## Addong Using

### Addong Using - Kodi Default Ski - TVShow View

- Leage Wideist:

<img height="600" src="_images/addon_view_league_widelist.jpg" alt="Kodi Adoon: The Sports Database Python - Leage Wideist">

- Leage Wall:

<img height="600" src="_images/addon_view_league_wall.jpg" alt="Addon Settings">

- League Shift:

<img height="600" src="_images/addon_view_league_shift.jpg" alt="Addon Settings">

- League Poster:

<img height="600" src="_images/addon_view_league_poster.jpg" alt="Addon Settings">

- League List:

<img height="600" src="_images/addon_view_league_list.jpg" alt="Addon Settings">

- League Infowall:

<img height="600" src="_images/addon_view_league_infowall.jpg" alt="Addon Settings">

- League Fanart:

<img height="600" src="_images/addon_view_league_fanart.jpg" alt="Addon Settings">

- League Banner:

<img height="600" src="_images/addon_view_league_banner.jpg" alt="Addon Settings">


### Addong Using - Kodi Default Ski - Season View

- Season Widelist:

<img height="600" src="_images/addon_view_season_widelist.jpg" alt="Kodi Adoon: The Sports Database Python - Leage Wideist">

- Season Wall:

<img height="600" src="_images/addon_view_season_wall.jpg" alt="Kodi Adoon: The Sports Database Python - Leage Wideist">

- Season Shift:

<img height="600" src="_images/addon_view_season_shift.jpg" alt="Kodi Adoon: The Sports Database Python - Leage Wideist">

- Season Poster:

<img height="600" src="_images/addon_view_season_poster.jpg" alt="Kodi Adoon: The Sports Database Python - Leage Wideist">

- Season List:

<img height="600" src="_images/addon_view_season_list.jpg" alt="Kodi Adoon: The Sports Database Python - Leage Wideist">

- Season Infowall:

<img height="600" src="_images/addon_view_season_infowall.jpg" alt="Kodi Adoon: The Sports Database Python - Leage Wideist">

- Season Fanart:

<img height="600" src="_images/addon_view_season_fanart.jpg" alt="Kodi Adoon: The Sports Database Python - Leage Wideist">

### Addong Using - Kodi Default Ski - Episode View 

- Episode Widelist:

<img height="600" src="_images/addon_view_episode_widelist.jpg" alt="Kodi Adoon: The Sports Database Python - Leage Wideist">

- Episode Wall:

<img height="600" src="_images/addon_view_episode_wall.jpg" alt="Kodi Adoon: The Sports Database Python - Leage Wideist">

- Episode Infowall:

<img height="600" src="_images/addon_view_episode_infowall.jpg" alt="Kodi Adoon: The Sports Database Python - Leage Wideist">

### Addong Using - Kodi Default Ski - Actor View 




:+1: Thank you for reading! :shipit: you can find me on discord!

:+1: Thanks also to ZAG, the operator of <a href="https://www.thesportsdb.com/">thesportsdb.com</a> which supports all Kodi and Plex users with its data. Helping hands are always needed for content creation, visit the Discord Channel: <a href="https://discord.gg/pFvgaXV">discord.gg/pFvgaXV</a>


> [!TIP]
> Support us on Patreon: patreon.com/ProjectKodi

