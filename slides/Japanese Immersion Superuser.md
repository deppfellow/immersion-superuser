# Japanese Immersion Superuser

## 1. Setup Your PC

Installing language, fonts, and setting up locale to Japan.
    1. Adding new language by simply open "Language settings" => "Add a language" in your Windows machine
    2. Get a fonts, personally I used [Noto Sans JP](https://fonts.google.com/noto/specimen/Noto+Sans+JP). Install as usual
    3. Setting Japanese Locale by administrator powershell, then run `Set-WinSystemLocale -SystemLocale ja-JP; Restart-Computer`


## 2. Setup Anki & Ankiconnect

Download Anki from [link](https://github.com/ankitects/anki/releases). Get addon below:
- 2055492159 [Ankiconnect](https://ankiweb.net/shared/info/2055492159)
- 759844606 [FSRS4Anki](https://ankiweb.net/shared/info/759844606)
- 1344485230 [AJT Japanese / Furigana, Pitch Accent, Native pronunciations](https://ankiweb.net/shared/info/1344485230)

- 757527607 [AutoReorder](https://ankiweb.net/shared/info/757527607)
- 291119185 [Batch Editing](https://ankiweb.net/shared/info/291119185)
- 874215009 [Advanced Browser](https://ankiweb.net/shared/info/874215009)
- 1898445115 [Advanced Copy Field](https://ankiweb.net/shared/info/1898445115)
- 385888438 [Edit Field During Review (Cloze)](https://ankiweb.net/shared/info/385888438)

- 1771074083 [Review Heatmap](https://ankiweb.net/shared/info/1771074083)
- 1247171202 [Study Time Stats](https://ankiweb.net/shared/info/1247171202)
- 738807903 [More Overview Stats 2.1](https://ankiweb.net/shared/info/738807903)
- 1779060522 [True Retention by Card Maturity Simplified](https://ankiweb.net/shared/info/1779060522)
- 1610304449 [Kanji Grid Kuuube](https://ankiweb.net/shared/info/1610304449)
- 266436365 [Progress Graphs](https://ankiweb.net/shared/info/266436365), `shift+click` to see graphs

- 1045800357 [Local Audio Server for Yomichan](https://ankiweb.net/shared/info/1045800357)
- 580654285 [Yomichan Forvo Server](https://ankiweb.net/shared/info/580654285)

All code download:
```
2055492159 759844606 1344485230 757527607 291119185 874215009 1898445115 385888438 1771074083 1247171202 738807903 1779060522 1610304449 266436365 1045800357 580654285
```

After that, changes Anki's default settings:
1. Turn on FSRS (pick one deck => "OPtions" => "Enable FSRS")
2. In "Daily Limits", set new cards/day to 20, and maximum reviews/day to 9999
3. In "New Cards", set learning steps to `1m 5m 1h`
4. In "Lapses", set relearning steps to `5m 1h`
5. In "Display Order", set new/review order to `Show before reviews`
6. in "FSRS", enable FSRS and set desired retention to `0.90`, then click "Optimize"
7. Don't forget to click "Save"


## 3. Setting up Yomitan

Use your preferred browser (e.g. Firefox, Chrome), and install Yomitan extension. Grab these [Yomitan's settings](#) and import from `Backup` => `Import Settings`. Then add dictionary, get from [shoui's collection](https://drive.google.com/drive/folders/1tTdLppnqMfVC5otPlX_cs4ixlIgjv_lH), including:
- [Bilingual] Jitendex, JMDict
- [Monolingual] 
    [実用日本語表現辞典](https://drive.google.com/file/d/1Szy4XWC6KEa2w7rVyjuJqxXuOfEnsjpr/view?usp=sharing) (Jitsuyou Nihongo Hyougen), 
    [旺文社国語辞典](https://drive.google.com/file/d/1x-lQ5lSVcyH_Nnh_NZyRVpkINg2Ez-PB/view?usp=sharing) (Oubunsha Kokugo), 
    [旺文社国語辞典 画像無し](https://drive.google.com/file/d/1WhJk0gsgL2z_A6cYqIB7185EZd5GPvxs/view?usp=sharing) (Oubunsha Kokugo・No Image version), 
    [三省堂国語辞典 第三版](https://drive.google.com/file/d/169tv6bKqqGuv8Y5Wj9f8SpP3IGxYZUKD/view?usp=sharing) (Sanseidou), 
    [明鏡国語辞典](https://drive.google.com/file/d/1touXH6uNsq41bYGU1xnB_lTFfrynerBU/view?usp=sharing) (Meikyou Kokugo), 
    [ハイブリッド新辞林](https://drive.google.com/file/d/1vsko6-vDDMDC2zp_BD0o99SHc0WoOR5U/view?usp=sharing) (Hybrid Shinjirin),
    [新明解国語辞典](https://drive.google.com/file/d/1M9qlt0hKVwyiyM7rqRPfi3nB_HTj2dOO/view?usp=sharing) (Shinmeikai Kokugo),
    [デジタル大辞泉](https://drive.google.com/file/d/1Mmr7IIy9CWv9YlCezrOE7JK-7PBV_CyI/view?usp=sharing) (Digital Daijisen)
- [Grammar] DoJG, Donna Toki dou Tsukau, Nihongo Kyoshi, E de Wakaru, Nihongo no Sensei
- [Names] JMnedict
- [Freq] JPDB, CC100, BCCWJ, VN, Narou, Novels, Anime & J-drama

Monolingual dictionaries is sorted based on personal recommendation, with exception of Digital Daijisen. Always get it since its has very wide words coverage.

### Difference between each frequency dictionaries
| Corpus | Freq Source | Focus |
| --- | --- | --- |
| JPDB | Mixed japanese media (e.g. anime, novels, vn) | Anime, drama, novels, VNs (i.e. any entertainment medias) |
| CC100 | Web pages in Japanse (from Common Crawl Project) | Interned-based Japanese (i.e. modern slang, informal wriing) |
| BCCWJ | Books, newspaper, legal docs, blogs, spoken dialoge | Balanced modern Japanese (academic study, general learners) |
| VN | Japanese visual novel | Learning from visual novels (good for storytelling and dialogue) |
| Narou | Web novels from "Shousetsuka no Narou" (i.e. sites for amateur novels) | Web novel fans |
| Novels | Published novels (i.e. light novels, traditional literature) | Literary Japanese (advanced learners, more kanji) |
| Anime & J-drama | Substitles from anime & drama | Natural spoken Japanese |


## 4. Setting Up MPV and Mpvacious for Video Mining

Under construction

## 5. Setting Up Visual Novel Mining

Install [Textractor](https://github.com/Artikash/Textractor), [ShareX](https://getsharex.com/), and [JL](https://github.com/rampaa/JL). For Textractor, set your extension to look like these:
```
- Remove Repeated Characters
- Remove Repeated Phrases
- Remove Repeated Phrases 2
- Extra newlines
- Regex Filter (optional, but needs to be above clipboard)
- Copy to Clipboard
- TextractorSender
- Google Translate (or any other translate. Optional, if you want to immediately translated hooked text)
```

For ShareX,
1. Start by import these [settings](https://mega.nz/file/UnUjUDzC#zlF_iuIdELDq4-rk4o20EYa4Be3qdc3y5Caay9Eumbg). Go to `Application settings...` > `Settings` > `Import`
2. Go to `Hotkey settings...`, and there will be four options.
    1. First is "Audio (Anki)", which will record an audio and sent directly to Anki's `collection.media`. Click on gear icon. In "Task", change the path at the most bottom to your own Anki's `collection.media` (usu. `C:/Users/<USERNAME>/AppData/Roaming/Anki2/<ANKIPROFILE>/collection.media`)
    2. Now, go to "Screen recorder", and open "Screen recording options". Click "Install recorder devices". Once done, click "Video source" and set to "None". Then click on "Audio source" and set to "virtual-audio-capturer".
