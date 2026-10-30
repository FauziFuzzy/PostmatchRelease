# Changelog

What changed in each version of Postmatch (called LastRound up to 1.0.6). To update, use the
Update button in the dashboard, or download the newest `Postmatch-Setup.exe` and run it over
your current version; your settings and recordings are kept.

## 1.3.9 - 2026-10-30

- **No more matches recorded many times over.** If Postmatch's background watcher stopped
  unexpectedly mid-game, the copy that restarted a few minutes later began a new recording but
  left the old one running. In one long Call of Duty session that added up to about 20
  recordings of the same match at once: hundreds of GB of duplicate pieces, a busy graphics
  card, and a match stuck on "Getting it ready" for good. A restart now ends the old recording
  first, so there is only ever one.
- **The log now says when the watcher stopped unexpectedly**, and when it was last seen
  running, to help track down why.

## 1.3.8 - 2026-10-30

- **Alt-tabbing no longer cuts your recording into pieces.** In some games (Call of Duty, for
  one), alt-tabbing out made Postmatch think the game had changed size, so it started a new
  piece each time: one evening's session became six pieces that then took a long time to join
  back together. Sometimes it stopped recording altogether. Now only a real change of
  resolution starts a new piece.

## 1.3.7 - 2026-10-29

- **Anonymous usage stats.** Postmatch now counts how often it's opened and which features get
  used (clips, trims, share links, posts, Team review), with a random id for your PC. It never
  sends your account, names, files or recordings. This shows what to improve next. Turn it off in
  Settings > About; the [privacy policy](https://postmatch.tv/privacy.html) lists what's sent.

## 1.3.6 - 2026-10-27

- **A match could get stuck on "Getting it ready".** If you started a new match while the last
  one was still being got ready, the two could trip over the same file and the newer match was
  never finished. Each match is now only ever handled by its own session. Anything stuck from
  before is finished the next time Postmatch starts.
- **See how long getting a match ready has left.** Every slow step now shows how far it has
  got and the time left: "Joining pieces 60% · 12 min left" (when the game's window changed
  size mid-match), "Finishing 40%", and "Compressing 25% · 7 min left". Joining used to show
  no progress at all.

## 1.3.5 - 2026-10-26

- **A smoother dashboard.** It no longer redraws the whole window every second while nothing
  is happening: only what changed is drawn again, like a recording timer, a new log line or a
  new clip. Sitting on Matches it now draws almost nothing.
- **Pages keep what they showed.** Coming back to the Feed or Team review shows your posts,
  squads and scrims straight away while they refresh, instead of loading from scratch. Signing
  out clears them.
- **Settings stay in step.** A change made elsewhere (another window, or Postmatch itself)
  shows in Settings while it's open.
- **A new network engine** for Team review and share-link uploads, the Discord server list and
  update checks.

## 1.3.4 - 2026-10-25

- **See how long a Team review upload has left.** The line under the scrim now ends with the
  time left: "copy ready in 9 min" while Postmatch makes the copy, then "2 min left" while it
  uploads.
- **Uploads no longer vanish when you switch pages.** Going to another page and back to Team
  review used to hide an upload in progress (it kept going, but you couldn't see or cancel
  it, and sharing again said a copy was being made already). Now its progress and Cancel are
  still there, and "Shared" or "Not shared" shows on whatever page you're on.

## 1.3.3 - 2026-10-25

- **Remove your POV from a scrim.** Once your POV is in, your seat in Team review shows a
  small x. Press it, say yes, and your video comes out of the scrim (and off Postmatch's
  storage) for the whole team, so you can add a different recording. The notes stay, and
  your recording stays on your PC.

## 1.3.2 - 2026-10-24

- **Sharper POVs in Team review.** The copy Postmatch uploads for your team is now 1080p
  instead of 720p, at a much higher quality: fire, smoke and grass no longer smear into
  blocks. Making the copy still takes about a minute for a match; the upload is about two
  and a half times bigger, so it takes longer on a slow connection. A very long session is
  made a little smaller, so it always fits in one upload.
- **Team review uploads stay in Team review.** Uploading your POV no longer shows as a
  banner on Clips, a row on Matches or the gold dot on Clips; its progress shows on your
  seat in Team review only.
- **Tidier Team review player.** Tagging players with long names no longer runs into the
  Add note button, and the time beside the bar no longer wraps or touches the playhead on
  matches over an hour.

## 1.3.1 - 2026-10-24

- **Play the part in Trim.** Play part plays your part from its start to its end, with the
  playhead following, straight from your recording. The small play buttons beside Set start
  and Set end play just its first or last 3 seconds, so you can check where it starts and
  stops. Space plays or pauses.
- **Move along a long match in Trim.** Scrolling over the filmstrip now moves along the match
  (Ctrl+scroll zooms, as scrolling did before), and a bar under it shows the whole match with
  your part and a box for what the filmstrip shows: drag the box, or click anywhere on the bar.
- **No more lag while moving through a match in Trim.** The pictures in the filmstrip and the
  big picture now load once you stop moving, instead of for every step on the way, which could
  make the whole PC stutter on a long match.
- **A new logo.** The pixel P now has one leg, with the play button beside it, so it no longer
  reads as an R. The sidebar logo reads POSTMATCH+ when you have Postmatch+.

## 1.3.0 - 2026-10-22

- **Team review, with scrims as folders.** Sign in, then create a squad (Postmatch+) or join one
  with its invite code (free): up to 5 players and a coach. Anyone makes a scrim for the next
  match: planned for later, playing now, or already played. After you play, press your seat on
  the scrim's card, or drag one of your recent recordings onto it. Add my POV picks the
  recording that fits the scrim's time, shows how it lines up with your teammates' POVs, and
  warns you if it's another game, day or time. It makes a 720p copy on your graphics card and
  uploads it while you keep playing. Every POV then plays in sync, side by side, with
  timestamped notes tagged to the players they're for; For me lists the ones for you. You hear
  live when a teammate's POV is in. The squad's captain gets a three-step setup (name, invite,
  first scrim), and players get a short welcome when they join.
- **Share links.** Any clip, or any part of a match from the trim editor, becomes a
  postmatch.tv link that plays right in Discord and on phones. Post to Discord sends the link.
  Free links last 30 days at up to 1080p.
- **The Feed.** A new page in the app: post your clips, and like, comment on and follow other
  players' posts. There's an Activity list, a search for players by name, and suggestions from
  your Discord servers. Report and block are in each post's menu.
- **Your profile** at postmatch.tv/u/you: picture, banner, bio and your share links. Edit it in
  Settings > Profile, from a picture, GIF, video, clip or match.
- **Postmatch+** ($4.99 a month or $47.88 a year, 14 days free): create your squad, share links
  kept forever at up to 1440p (100 GB), an animated profile picture and banner, the PLUS badge,
  and your own hotkey sounds. Hotkey sounds play only in your headset and are left out of the
  recording. Manage or cancel it in Settings > Postmatch+.
- Times in Team review are shown 12-hour, like the rest of the app.

## 1.2.10 - 2026-10-22

- **Sign in with Google or Discord.** A new account screen, over a slowly drifting wall of game
  art, opens once before setup on a new install and any time from Settings > Account. Continue
  with Google or Discord opens your browser, and Postmatch comes back to the front once you're
  signed in; you stay signed in until you sign out in Settings > Account. Your rank on every PC,
  Team review and clip links will use it. "Continue without an account" makes a guest account
  instead; signing in later keeps it.
- **Post clips to Discord by themselves.** Paste a channel's webhook in Settings > Discord
  (Server Settings > Integrations > Webhooks > Copy Webhook URL) and turn on "Post new clips
  automatically": every clip you make and every moment you save with F8 goes to that channel
  once your match has ended, with the game and match it's from - as a copy Discord plays right
  in the chat. Any clip also has Share > Post to Discord, with its progress on the clip's row.
  Each post reads "**Fuzzy** shared a clip from BF6 | Recorded with #Postmatch" (your name in
  posts is in Settings > Discord), then the video, then a Postmatch card with the clip, the match it's from and its
  length. Send logs leaves the webhook out.
- **Trim a match.** A match's new Trim button (or "Trim or share a part..." in its menu) opens
  a filmstrip editor, on your first F9 mark (or the loudest moment). A big picture shows the
  playhead; below it, a strip of pictures with the match's sound and your marks, where purple
  handles set the part - click to move the playhead, scroll to zoom out to the whole match.
  I / O set the start / end at the playhead, the arrow keys move it a second. Then save it as:
  - **Full quality** - any length, starting exactly where you put it, with its size shown; it
    shows in Clips, tagged TRIM.
  - **Discord copy** or **Post to Discord** - up to 2 minutes, under Discord's 10 MB. The
    editor says how sharp it will be (a 20-second part is 1080p, 90 seconds 360p).

  The editor stays open while it works: its button fills up and says what's happening
  ("Uploading 63%"), then how it went, so you can go straight on to the next part.
- The clip menu's "Discord size" option and the match menu's "Copy file path" are gone; ticked
  clips still have Copy for Discord.

## 1.2.9 - 2026-10-21

- **Your rank keeps what you've played.** Deleting a recording no longer lowers your rank or
  your stats: Postmatch keeps a career of every match it has finished, and the first time it
  rebuilds that history from its log - so matches you deleted before count again.
- **Times are 12-hour:** a match started at 20:01 now shows 8:01 PM, everywhere in the dashboard.

## 1.2.8 - 2026-10-21

- **See how far compressing has got.** A match that's getting ready after you play now shows
  "Compressing 42%" with a bar that fills up, in the list and in the big preview, updated every
  few seconds.

## 1.2.7 - 2026-10-21

- **Fixed: "Getting it ready" ran past the thumbnail** in a narrow window. A small thumbnail
  now says "Getting ready..." on one line.

## 1.2.6 - 2026-10-21

- **Fixed: your voice was missing when playing a recording.** The game sound and your mic were
  recorded as two tracks, and players (and clips) only played the first. After each match they
  are now one track, game and mic together, with a quiet mic raised (up to 12 dB) so your voice
  is clear over the game. Clips, saved moments (F8) and Discord copies have your voice too.
- **Every game records at 60 fps, the whole match.** No more light mode switching to 30 by
  itself when memory was nearly full. Settings > Frame rate: 60 fps (the default) or 30 fps,
  your choice.
- **Quality picked for your PC.** Setup checks your graphics card and memory and suggests a
  quality: High (your game's resolution, 25 Mbps) for a gaming card with 16 GB or more,
  Balanced (up to 1080p, 16 Mbps) for less memory or an entry-level card, Light (up to 720p,
  10 Mbps) for built-in graphics or a PC without a graphics-card encoder. The picture is scaled
  down on the graphics card. Settings > Quality: Automatic, or any of the three.
- **Stats is a ranked career now.** Every minute you record earns 1 RP and climbs you through
  seven ranks, Rookie to Immortal, each with divisions III, II and I. The page shows your
  rating and rank, how it climbed this week or season, your top games and your streak.
- **Settings, redesigned.** Sections down the left (Recording, Audio, Hotkeys, Games, Storage,
  Advanced, About), one row per setting, and changes save by themselves.
- **Setup's last step has a little pixel gamer** ready to go. Setup also keeps your recordings
  folder when you look at another drive and come back.
- **The game filter no longer gets cut off.** When the game chips don't fit across Matches or
  Clips, they become one Game menu.
- The Game and sort menus' highlight now has rounded corners like the buttons.

## 1.2.5 - 2026-10-21

- **Games running faster than 120 fps keep more of their fps.** Windows used to copy every
  frame a game drew for the recorder, which only keeps 60 a second - at 600 fps in Valorant
  that was ~540 copies a second thrown away, and cost the game ~100 fps. The recorder now takes
  at most 120 pictures a second, in window and screen capture alike.

## 1.2.4 - 2026-10-20

- **No more live preview picture** on the Record page. The recorder no longer copies a picture
  back from the graphics card for it, and holds one frame fewer in video memory. The live
  numbers (frames per second, file size, bitrate, sound meter) stay.

## 1.2.3 - 2026-10-20

- **Fixed: recordings looked like 30 fps** with Frame rate on Automatic. Light mode went on
  whenever a game pushed the CPU or GPU past 90% - which is normal for any game running as fast
  as it can - and could stay on for most of a match. It now only goes light when memory is nearly
  full (94%+, when Windows starts swapping and games stutter), and comes back as soon as memory
  frees up.

## 1.2.2 - 2026-10-20

- **Recording adapts to your PC by itself.** Frame rate is now Automatic: Postmatch watches
  how busy the CPU, GPU and memory are, and while a game maxes your PC out it records a new
  picture every other frame (light mode) so the game stays smooth, then goes back to full 60 when
  things calm down. The Record page shows "Light mode · PC busy" meanwhile. Always 60 or always
  30 fps can still be picked in Settings.
- **Lighter recording of fast games.** A game running faster than 60 fps (150+ with frame
  generation) no longer has every frame copied - only the ones the recording uses.
- **The game draws first.** The recorder's GPU work runs at lower priority than the game, and
  holds fewer frames in video memory.
- **Fixed: compressing to H.264 could drop a few frames** (6 in 2400 in a test).

## 1.2.1 - 2026-10-20

- **Fixed: Send logs made a zip that looked empty** in Explorer. It now also includes the
  watcher's own log and the PC's CPU, memory and graphics cards with their driver versions.
- **Capture setting.** Settings > Disk and capture: Automatic (the game's window on Windows 11,
  the screen on Windows 10), Game window, or Screen - to compare if recording feels heavy.
- **Lighter capture.** The recorder reuses its picture buffers instead of making a new one for
  every frame.

## 1.2.0 - 2026-10-20

- **Save the last 30 seconds: F8.** While a game records, press F8 (or "Save last 30 s" on the
  Record page) and the last 30 seconds go straight into Clips as a lossless copy, tagged SAVED.
  Postmatch only notices the key - your game still gets it.
- **Mark a moment: F9.** A gold tick on the match's timeline where you pressed it.
- **Match timeline.** Every new match shows the game sound's loudness over the whole match, with
  your marks in gold and its clips as dots. Make clips also gets faster: it uses the loudness
  measured while recording instead of reading the whole match again.
- **Live recording view.** The Record page shows what's being recorded (a picture every 3 s) and
  live numbers: frames per second, skipped frames, file size so far, bitrate and a sound meter.
- **Hotkeys in Settings.** Pick other keys, or turn them off, and how much "save" keeps (15 s to 2 min).
- **Always records on the graphics card.** Postmatch now picks the GPU with a hardware video
  encoder itself - on gaming laptops the NVIDIA/AMD chip, not the built-in one - instead of
  Windows' default, which could leave the CPU encoding. The Record page shows "GPU", and warns if a
  PC has no GPU encoder at all. Clips use the GPU through Windows' own encoder too.
- **Lighter live preview.** The preview picture is only made while the Record page is open.
- **Compressing after a match barely touches the CPU.** It now decodes on the graphics card too,
  so the video never leaves the GPU: about a twelfth of the CPU it used (it could keep 4 cores busy
  before). Compressing and making clips also run at low priority, so a game always comes first.
- **Cancel compressing.** A match that's "getting ready" has a Cancel button: compressing stops
  and the recording is kept as recorded (bigger, but ready right away).

## 1.1.0 - 2026-10-19

- **LastRound is now Postmatch.** New name and a new logo: an 8-bit P with a play button in
  purple and cyan. Installing Postmatch replaces LastRound: it stops it, removes its program
  folder and shortcuts, and brings your settings, games, logs and thumbnails over on the first
  start. Your recordings are not moved: if you never picked a recordings folder, Postmatch keeps
  recording into `Videos\LastRound` so everything you have still shows in the dashboard.
- **Updating from LastRound works as usual.** LastRound's Update button (1.0.4 and later) offers
  this version and installs Postmatch over it in one click. The releases now live at
  `FauziFuzzy/PostmatchRelease`; old LastRound links still lead there.
- **A new dashboard.** A fresh look throughout, and the window opens at a comfortable size.
  New **Record** page: the live recording, today's matches and your capture settings at a glance.
- **Matches, side by side.** Your matches on the left, grouped by day; click one to see it on
  the right with Review, Make clips and Discord, plus every clip made from it. Clicking a match
  responds straight away. With more than five games, the game chips become one Game menu with
  a count per game.
- **Clips as a list.** One row per clip with its game, length, size and date, and its own
  Delete button. Tick several to make Discord copies or move them to the Recycle Bin together.
  Search and sort work on Clips too.
- **Game icons.** Every game shows its own icon, taken from the game's program file (or Steam's
  icon when the program has none). Pick your own picture for a game in Settings > Games.
- **Setup when you first install.** Five quick steps: your games (Postmatch scans your PC for
  installed ones), your microphone, video quality, which drive to record to, and a summary.
- **Settings, redesigned** into clear sections, with the recordings folder picked by button.
- **Coming soon, marked as such:** match results (win/loss, K/D/A), auto-clipped moments,
  hotkeys, team review and public clip links show in the app with a "Soon" tag.

## 1.0.6 - 2026-10-19

- **Fixed:** Settings > Change... closed LastRound's dashboard instead of opening the folder
  picker (1.0.5).

## 1.0.5 - 2026-10-19

- **Discord size.** A Discord button on every clip (and on recordings up to 2 minutes) makes a
  copy under Discord's 10 MB upload limit and shows it in Explorer, ready to drag into a chat.
  A 45-second clip comes out around 9 MB in a few seconds.
- **Send logs.** Settings > Send logs saves LastRound's logs and your PC's details (Windows
  version, graphics encoders, microphones, settings) in one zip to send to whoever helps you.
  Nothing is uploaded.
- **Choose the recordings folder with a button.** Settings > Change... opens Windows' folder
  picker instead of typing a path.

## 1.0.4 - 2026-10-19

- **Update button.** The dashboard tells you when a new version is out (sidebar icon and
  Settings > Updates) and installs it in one click: it downloads the installer, checks it
  matches the release, installs it and reopens LastRound. It never updates while a game is
  recording. This is the only thing LastRound fetches from the internet: one small request to
  GitHub when the dashboard opens and every 6 hours.
- **Choose your microphone.** Settings > Microphone: Windows' default, a specific mic, or off.
  If the chosen mic is unplugged, Windows' default is used until it's back.
- **No yellow border on Windows 10.** Windows 10 always draws a yellow border around a window
  that's being captured. On Windows 10 LastRound now records the game's area of the screen
  instead, without a border. While the game isn't in front (alt-tab), that part of the video
  is black, so nothing else on your screen is recorded. Windows 11 keeps recording the game
  window, with the border hidden.

## 1.0.3 - 2026-10-19

- **Recordings play in every player**, including Windows Media Player. LastRound saves the
  smallest format (HEVC) only on PCs that can play it (with Microsoft's HEVC Video
  Extensions), and H.264 otherwise: about a third bigger at the same quality.
  Settings > Video format lets you choose.
- **Your games are found automatically.** No built-in game list any more: play a game
  fullscreen once and it's added to Settings, then recorded in any window mode. Games are
  recognised from Steam, Epic, Riot, Xbox, EA, Ubisoft, GOG, Amazon and Rockstar folders, and
  from Windows' own list of games, wherever they're installed.

## 1.0.2 - 2026-10-19

- **Clips work again.** Every clip failed in 1.0.0 and 1.0.1.
- **Yellow border on Windows 11:** LastRound now asks Windows for permission to hide it. If
  it still shows, allow desktop apps under Settings > Privacy & security > Screenshot borders.

## 1.0.1 - 2026-10-19

- Clips are cut and framed 9:16 without captions. Captions needed Python, which most PCs
  don't have.

## 1.0.0 - 2026-10-19

- First public release: automatic recording of every game, HEVC compression on your GPU, a
  game-library dashboard, and 9:16 clips of your loudest moments.
