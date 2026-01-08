# DSR Media Server (Cloudflare Pages)

This project provides a permanent public URL for a local HTTP media server
using Cloudflare Pages as a reverse proxy.

## How it works
- Cloudflare Pages hosts a permanent website
- All requests are proxied to a temporary TryCloudflare URL
- When the TryCloudflare link changes, only `_redirects` needs updating

## Files
- `_redirects` → handles proxying to the TryCloudflare link
- `index.html` → placeholder page for deployment

## Update TryCloudflare URL
1. Open `_redirects`
2. Replace the old TryCloudflare link with the new one
3. Commit changes
4. Cloudflare Pages auto-deploys

## Example
Permanent URL:
https://dsr-media-pages.pages.dev

Proxied target:
https://experience-jackets-warnings-improvement.trycloudflare.com

## Notes
- Supports audio, video, images, and folders
- Free and fast using Cloudflare network
