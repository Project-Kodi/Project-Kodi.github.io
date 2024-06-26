
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

  - Preferred language (Fallback EN): Title/description and other texts are retrieved in this selected language.

- Trailer

  - Enable Trailer: Is for episodes only, information is already stored in Kodi, but trailers are not yet supported for episodes.

  - Addon Player: Used for playing the trailer (not used at this time)

- API:

  - TSDB - API Version: Here you can switch between the API versions. You only get the latest features with version 2.

  - Sleep in seconds each API call: Since only 100 requests are allowed per minute, you need at least 0.1 seconds delay. (Fast server/workstations)

<img height="600" src="_images/addon02.jpg" alt="Addon Settings">

### Addon Settings - NFO

- Scraper

  - Ignore local NFO file: With Kodi you can't turn off the search for NFO files, but you can bypass it. The NFO file must contain at least one of the following tags with data. Example <tsdb>4234</tsdb> or <episodeguide>{tsdb:4234}</episodeguide>. Tags: <title>, <showtitle>, <originaltitle>, <strLeague>, <tsdb>, <episodeguide> and <tvshowsource>.

> [!TIP]
> Before scraping the first time, you should remove any existing NFO files in your Sports Series folder.
> Kodi then always fetches the most current data from the Internet, even if an NFO file has been saved.

- NFO

  - x

    - y

  - x

  - x

  - x

<img height="600" src="_images/addon03.jpg" alt="Addon Settings">

<img height="600" src="_images/addon04.jpg" alt="Addon Settings">


### Addon Settings - Modifications 

- Title

<img height="600" src="_images/addon05.jpg" alt="Addon Settings">




### Addon Settings - Artwork 

- TVShows

- Seasons

- Character Art (Player)


<img height="600" src="_images/addon06.jpg" alt="Addon Settings">


<img height="600" src="_images/addon07.jpg" alt="Addon Settings">


### Addon Settings - Logging & Other

- Logging

- Premium 

- Support

<img height="600" src="_images/addon08.jpg" alt="Addon Settings">



## Addong Using

### Addong Using - xyz 

bla bla

### Addong Using - dsa 

bla bla

### Addong Using - qwe 

bla bla



:+1: thank you for reading! :shipit:


> [!TIP]
> Support us on Patreon: patreon.com/ProjectKodi

