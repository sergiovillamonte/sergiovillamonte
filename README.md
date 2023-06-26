- 👋 Hi, I’m @sergiovillamonte
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on a bug (youtube-dl)...
- 📫 How to reach me ...

<!---
sergiovillamonte/sergiovillamonte is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
this is the youtube-dl output
youtube-dl https://www.youtube.com/watch?v=_RL-l8YzkRo --verbose
[debug] System config: []
[debug] User config: []
[debug] Custom config: []
[debug] Command-line args: ['https://www.youtube.com/watch?v=_RL-l8YzkRo', '--verbose']
[debug] Encodings: locale UTF-8, fs utf-8, out utf-8, pref UTF-8
[debug] youtube-dl version 2021.12.17
[debug] Python version 3.10.6 (CPython) - Linux-5.15.0-75-generic-x86_64-with-glibc2.35
[debug] exe versions: ffmpeg 4.4.2, ffprobe 4.4.2, rtmpdump 2.4
[debug] Proxy map: {}
[youtube] _RL-l8YzkRo: Downloading webpage
[youtube] _RL-l8YzkRo: Downloading MPD manifest
ERROR: Unable to extract uploader id; please report this issue on https://yt-dl.org/bug . Make sure you are using the latest version; see  https://yt-dl.org/update  on how to update. Be sure to call youtube-dl with the --verbose flag and include its complete output.
Traceback (most recent call last):
  File "/usr/lib/python3/dist-packages/youtube_dl/YoutubeDL.py", line 815, in wrapper
    return func(self, *args, **kwargs)
  File "/usr/lib/python3/dist-packages/youtube_dl/YoutubeDL.py", line 836, in __extract_info
    ie_result = ie.extract(url)
  File "/usr/lib/python3/dist-packages/youtube_dl/extractor/common.py", line 534, in extract
    ie_result = self._real_extract(url)
  File "/usr/lib/python3/dist-packages/youtube_dl/extractor/youtube.py", line 1794, in _real_extract
    'uploader_id': self._search_regex(r'/(?:channel|user)/([^/?&#]+)', owner_profile_url, 'uploader id') if owner_profile_url else None,
  File "/usr/lib/python3/dist-packages/youtube_dl/extractor/common.py", line 1012, in _search_regex
    raise RegexNotFoundError('Unable to extract %s' % _name)
youtube_dl.utils.RegexNotFoundError: Unable to extract uploader id; please report this issue on https://yt-dl.org/bug . Make sure you are using the latest version; see  https://yt-dl.org/update  on how to update. Be sure to call youtube-dl with the --verbose flag and include its complete output.
