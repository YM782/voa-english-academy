# VOA English Academy

A personal offline-oriented study site for VOA Learning English:

- Level 1: 52 lessons
- Level 2: 30 lessons

## Current import status

- Level 1 lessons 1–46: transcript JSON files imported.
- Level 1 lessons 47–52: not yet imported.
- Level 2 lessons 1–30: not yet imported.
- Each imported lesson records its official VOA page and official MP3 URL. Lesson 45 includes a third-party song performance; its lyrics are omitted and its MP3 is excluded from the offline-cache batch pending separate rights clearance.
- MP3 files are downloaded on demand into the browser's separate Cache Storage using the site's sequential cache control. They are not currently committed as MP3 binaries in this GitHub repository.
- Offline playback has been user-tested successfully for Level 1 Lesson 4. Other lessons must be cached and tested individually or through the sequential batch action.

## Offline behavior

The service worker precaches the site shell and imported lesson JSON files. Audio is downloaded one file at a time to a separate persistent browser cache. The batch action skips audio already present in that cache and stops on the first failure to avoid uncontrolled data use. Browser cache is local to the browser profile/device; clearing site data or browser storage can remove it.

## Deployment

GitHub Pages: Settings > Pages > Deploy from a branch > `main` > `/(root)`.

## Source and reuse

Source credit: **VOA Learning English — https://learningenglish.voanews.com/**.

VOA Learning English states that its own texts, MP3s, photos and videos are in the public domain and may be reprinted for educational and commercial purposes with credit to learningenglish.voanews.com. This does not extend to third-party material embedded in VOA pages (for example, material credited to news agencies or other rights holders). Third-party material is excluded from this project unless its reuse rights are separately verified.

Official course catalogues:
- Level 1: https://learningenglish.voanews.com/p/5644.html
- Level 2: https://learningenglish.voanews.com/p/6765.html

This is an independent personal learning index and is not an official VOA website.
