# Audica Custom Difficulty Names
A mod that allows map makers to override the names of the map difficulties
 
## Installation
* Download MelonLoader from [here](https://github.com/HerpDerpinstine/MelonLoader/releases/latest)
* Download CustomDifficultyNames from [here](https://github.com/octoberU/SongBrowser/releases/latest)
* Put the **CustomDifficultyNames.dll** into Audica/Mods

## Changing difficulty names in your map
* Open the **song.desc** file in a text/code editor
* Add entries to the file for each custom name as follows
<pre><code>"customExpert" : "YOUR NAME HERE",
"customAdvanced" : "YOUR NAME HERE",
"customModerate" : "YOUR NAME HERE",
"customBeginner" : "YOUR NAME HERE"
</code></pre>

### Example of full song.desc
<pre><code>{
  "songID": "Mirror-MeepsKitten",
  "moggSong": "song.moggsong",
  "moggMainSong": "song.mogg",
  "title": "Mirror",
  "artist": "Porter Robinson",
  "midiFile": "song.mid",
  "fusionSpatialized": "fusion/guns/default/drums_default_spatial.fusion",
  "fusionUnspatialized": "fusion/guns/default/drums_default_sub.fusion",
  "targetDrums": "",
  "sustainSongRight": "",
  "moggSustainSongRight": "",
  "sustainSongLeft": "",
  "moggSustainSongLeft": "",
  "fxSong": "song_extras.moggsong",
  "moggFxSong": "song_extras.mogg",
  "tempo": 150.0,
  "songEndEvent": "event:/song_end/song_end_C#",
  "prerollSeconds": 0.5,
  "useMidiForCues": false,
  "hidden": false,
  "author": "MeepsKitten",
  "offset": 0,
  "previewStartSeconds": 27,
  "bookmarks": [],
  "customExpert" : "YOUR NAME HERE",
  "customAdvanced" : "YOUR NAME HERE",
  "customModerate" : "YOUR NAME HERE",
  "customBeginner" : "YOUR NAME HERE"
}
</code></pre>