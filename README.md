# Audica Custom Difficulty Names
A mod that allows map makers to override the names of the song difficulties

## Song Browser Users
In future [Song Browser](https://github.com/octoberU/SongBrowser) releases (Newer than v2.0.1) this mod's functionality will be included automatically.

<b>You do not need this mod if you have an installation of Song Browser newer than v2.0.1</b>

## Installation
* Download MelonLoader from [here](https://github.com/HerpDerpinstine/MelonLoader/releases/latest)
* Download CustomDifficultyNames and [SongDataLoader](https://github.com/MeepsKitten/CustomSongDataLoader) from [here](https://github.com/meepsalot69/Audica-CustomDifficultyNames/releases/latest)
* Put **CustomDifficultyNames.dll** and **SongDataLoader.dll** into Audica/Mods

## Changing difficulty names in your map
* Open the **song.desc** file in a text/code editor
* Add entries to the file for each custom name as follows
<pre><code>"customExpert" : "YOUR NAME HERE",
"customAdvanced" : "YOUR NAME HERE",
"customModerate" : "YOUR NAME HERE",
"customBeginner" : "YOUR NAME HERE"
</code></pre>

**Note**: some characters (like quotation marks) require an escape character ('/' in this case) to be able to be added to song.desc. If you don't do this your song will not load in game.

Example:
<code>"customAdvanced" : "this is how you escape a character /" see, not too hard"</code>

This would result in a difficulty that displays as <code>this is how you escape a character " see, not too hard</code>

You can use [this tool](https://www.freeformatter.com/json-escape.html) to see what characters are reserved and to automatically apply escape characters to any text.

**Advanced**: You can add [formatting tags](http://digitalnativestudios.com/textmeshpro/docs/rich-text/) to custom names. Any Text Mesh Pro tag should work.

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
