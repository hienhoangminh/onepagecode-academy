# OnePageCode Academy

A free learning companion for public OnePageCode YouTube playlists. Videos remain embedded from YouTube; no video files are downloaded or rehosted.

## Local development

```bash
npm install
npm run dev
```

## Import the catalogue

1. Enable YouTube Data API v3 in Google Cloud and create an API key.
2. Add it to this repository as an Actions secret named `YOUTUBE_API_KEY`.
3. Run **Build and deploy academy** in GitHub Actions. The script paginates channel playlists and playlist items, writing `src/catalog.json`.

YouTube API quota applies. Without the key, the app builds but its course list remains empty.

## Publish

In repository Settings → Pages → Build and deployment, select **GitHub Actions**. Intended URL: https://hienhoangminh.github.io/onepagecode-academy/.

## Scope

One public playlist becomes one course, in playlist order. Learners can open lessons in any order; completion is self-reported and stored in browser local storage. Quizzes, graded assignments, accounts, cross-device sync and verifiable certificates are not implemented in this initial scaffold; lesson activities must be grounded in reliable source material. Do not bypass Learn gates, copy gated resources, or automate extraction contrary to site terms; obtain permission before indexing third-party course resources.
