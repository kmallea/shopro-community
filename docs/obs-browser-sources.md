# OBS Browser Sources

ShoPro can publish live graphics to OBS through browser-source URLs. Supported experiences include tickers, chyrons or topic graphics, rundowns, and themed overlays.

## Add a source to OBS

1. Open **Sources** in ShoPro.
2. Create or select the graphic you want to use.
3. Copy its browser-source URL.
4. In OBS, open the destination scene.
5. Add a new **Browser** source.
6. Paste the URL.
7. Set the width and height to match your canvas or graphic design.
8. Position and crop the source as needed.
9. Trigger a test update from ShoPro before going live.

## Recommended setup

- Give each graphic a clear OBS source name.
- Keep browser sources in a dedicated scene when they are reused.
- Confirm text size and safe margins at the final stream resolution.
- Test long titles, ticker text, and multiple rundown items.
- Verify transparency and background colors.
- Check whether the source should shut down when hidden.

## Source security

Treat a complete browser-source URL as private. Anyone with the full URL may be able to display that production feed. Do not include source URLs in public bug reports or screenshots.

## When a source does not update

1. Confirm the ShoPro show is active and the correct source was copied.
2. Refresh the OBS browser source.
3. Check that OBS can reach `shopro.live` over HTTPS.
4. Confirm firewall, VPN, DNS, and proxy settings allow WebSocket traffic.
5. Open the source URL in a normal browser to isolate an OBS-specific problem.
6. Recreate the source only after recording its existing dimensions and settings.

See [Troubleshooting](troubleshooting.md) for more checks.
