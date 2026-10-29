# CuePlay

**Track movies, series and anime in one app — with friends, shared lists and chat.**

CuePlay is a free, open-source Android tracker for movies, TV series and anime from any country. It works fully offline with no account, and adds an optional social layer when you want one. No Google services, no ads, no analytics.

> **Status:** in early development. A beta is planned on GitHub Releases and IzzyOnDroid, followed by F-Droid.

## Features

**Tracking**
- One search across movies, series and anime
- Statuses: Watching, Plan to Watch, Completed, On Hold, Dropped, Rewatching
- Episode-by-episode progress grouped by season, with rewatch counts
- Scores from 1 to 10 and private notes
- Episode alerts for titles you're watching
- Works fully offline; no account required

**Lists and imports**
- Custom named lists with Public, Friends-only or Hidden visibility
- Import from MyAnimeList (XML) and IMDb (CSV)
- Two-way AniList account sync

**Social** (optional account)
- Friends, profiles and QR-code friend adding
- Activity feed with reactions and comments
- Send recommendations and see your taste match with each friend
- One-to-one chat with title cards, alerts via [UnifiedPush](https://unifiedpush.org/)
- Block, report and fine-grained privacy settings

**Premium** — a $2.99 one-time lifetime purchase
- Full library cloud sync and backup
- Stats, yearly recap, home screen widget and upcoming calendar
- Extra theme variants and app icons

**Languages:** English, Bangla, Hindi, Urdu, Arabic, Spanish, Portuguese, Indonesian, French and Japanese, with full right-to-left support.

## Privacy

- Your library lives on your phone. Nothing is sent to a server unless you create an account.
- No Google Play Services, Firebase, Crashlytics, AdMob or any proprietary SDK.
- No analytics or tracking.
- Private notes and hidden lists never leave your phone (unless you turn on premium sync).
- Deleting your account deletes all of your server data.

## Tech stack

| Area | Choice |
| --- | --- |
| App | Kotlin, Jetpack Compose |
| Local storage | Room (SQLite) |
| Backend | [Supabase](https://supabase.com/) (Postgres, Auth, Realtime, Storage) |
| Catalog proxy | Cloudflare Workers |
| Push | UnifiedPush |
| Payments | Paddle |

## Data sources

Movie and series data comes from [TMDB](https://www.themoviedb.org/); anime data comes from [AniList](https://anilist.co/). All catalog requests go through a CuePlay proxy, so no API keys live in the app or this repository.

This product uses the TMDB API but is not endorsed or certified by TMDB.

## Contributing

CuePlay is not ready for code contributions yet. Once the beta is out, issues, bug reports and translations (via Weblate) will be very welcome.

## Support

Questions or problems? Email **mdliad.se@gmail.com**.

## License

CuePlay is free software, released under the [GNU General Public License v3.0](LICENSE).
