microprofilecsv is a small tool for visualizing and comparing data coming from .csv files.

![](demo-video/demo.gif)

It spawned as a small hack from [microprofile](https://github.com/jonasmr/microprofile), and has now turned into its own little useful thing.


# Usage

* Open `microprofilecsv.html` in chrome
* Drag one or more .csv files onto the web page
	* If you drag more than one, they will be treated as a set, letting you visualize min/max/avg
	* A video can be included as well(mp4 or webm)
		* By default video will be mapped linearly: first csv row is the start of the movie, last row is the end
		* If there is one of two specific columns, these will used to control the position of the movie:
			* `time`: will be interpreted as the absolute time in **seconds** for each row
			* `frametime`: will be interpreted as frametime in **milliseconds**. Summed while parsing the file to derive the absolute time for each row.
* The Source menu can be used to control what is shown in each graph
* Mode Menu Controls what kind of graphs to show
* Preset menu can be used to save presets
	* Settings are saved and kept as long as the file is in the same position
* Set menu appears when you've dropped more than one set of csv files, and lets you control which one is drawn

# Shortcuts

* h: Show help
* 1-8: Set number of graphs
* Mousewheel or ctrl + mouse up/down: Zoom
* Mousewheel/Ctrl + mouse up/down: Zoom
* Left Mouse + mouse left/right: Pan
* Right Mouse + mouse left/right: Show Range info
	* Esc. to remove selection
* Space: Toggle Set display
* Hold z: Enlarge video and only show 1 graph


