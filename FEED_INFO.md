# Jim Rutt Show Feed - Quick Reference

## ✅ Your Feed is Live!

**Feed URL:** https://andrewblevins.github.io/jim-rutt-show-feed/substack_feed.xml

**GitHub Repo:** https://github.com/andrewblevins/jim-rutt-show-feed

---

## Next Steps for Substack Import

### 1. Validate the Feed (Recommended)
Go to: https://validator.w3.org/feed/

Paste your feed URL: `https://andrewblevins.github.io/jim-rutt-show-feed/substack_feed.xml`

### 2. Test in a Feed Reader (Optional)
Try in Feedly, NewsBlur, or any RSS reader to see how episodes display.

### 3. Import to Substack

**Option A: RSS Import (if Substack supports it)**
- Log into Substack
- Go to Settings → Import
- Look for "RSS feed" or "Podcast feed" import
- Enter: `https://andrewblevins.github.io/jim-rutt-show-feed/substack_feed.xml`

**Option B: Contact Substack Support**
If they don't have automated RSS import, send them:
- Feed URL: `https://andrewblevins.github.io/jim-rutt-show-feed/substack_feed.xml`
- Tell them: "Enhanced podcast feed with 443 episodes, including full show notes with hyperlinks"

### 4. Test First!
Consider importing to a Substack test account first, or ask Substack to import just 5-10 episodes initially.

---

## Feed Contents

- **443 episodes** (July 2019 - November 2025)
- **4,245 hyperlinked references** in show notes
- **413 transcript links**
- **557 book recommendations** (Goodreads)
- Full episode metadata (audio URLs, durations, dates)
- Organized show notes categories

---

## Updating the Feed

If you need to update the feed in the future:

```bash
cd /Users/andrew/jim-rutt-show/jim-rutt-show-feed
# Replace substack_feed.xml with new version
git add substack_feed.xml
git commit -m "Update feed"
git push
# Wait ~1 minute for GitHub Pages to rebuild
```

---

## Troubleshooting

**If Substack says feed is too large:**
- Let me know and I can split it into smaller feeds
- Or provide episodes in batches

**If Substack has format requirements:**
- We have all the data in JSON format
- Can generate any format they need
- Scripts are available in `/Users/andrew/jim-rutt-show/rss-feed-upgrade/`

**If links aren't working:**
- All 4,245 links have been tested and extracted
- May need minor HTML adjustments for Substack's renderer

---

## Technical Details

- **Hosting:** GitHub Pages (free, unlimited, fast CDN)
- **Format:** RSS 2.0 with content:encoded for HTML
- **Size:** 3.2 MB (no file size limits on GitHub Pages)
- **Uptime:** 99.9%+ (GitHub infrastructure)
- **HTTPS:** Yes (automatic)
- **Cost:** Free forever

---

## Questions?

All source files and scripts are in:
- Feed generation: `/Users/andrew/jim-rutt-show/rss-feed-upgrade/`
- This repo: `/Users/andrew/jim-rutt-show/jim-rutt-show-feed/`

Can regenerate or modify feed anytime with the Python scripts.

