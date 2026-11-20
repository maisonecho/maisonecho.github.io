# ViceTaped site (static)

Pages: `/` (index.html), `/terms` (terms.html), `/privacy` (privacy.html). Deployed on Vercel as a static site.

## TikTok URL verification (URL properties)
* **Signature file:** TikTok gives you a file like `tiktokXXXXXXXX.txt`. Run `./add_tiktok_verification.sh path/to/tiktokXXXXXXXX.txt`
  (copies it into the site root) and redeploy. It will be served at `https://<site>/tiktokXXXXXXXX.txt`.
* **Meta tag:** run `./add_tiktok_verification.sh --meta 'tiktok-developers-site-verification=XXXX'` and redeploy;
  the tag is added to the `<head>` of every page (replaces the `<!-- TIKTOK_VERIFY_META -->` marker).
