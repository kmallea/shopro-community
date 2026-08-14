# Using ShoPro with OBS

ShoPro integrates with OBS in two different ways:

- A **Custom Browser Dock** puts the ShoPro controls inside OBS so you can run the show without switching windows.
- A **Browser Source** displays ShoPro graphics such as tickers, chyrons or topic graphics, rundowns, and themed overlays in the program output.

The dock is your private control panel. Browser sources are visual layers intended for your OBS scenes.

## Add ShoPro as an OBS dock

Adding ShoPro as a Custom Browser Dock gives you access to the show planner and Run Mode directly inside OBS.

1. Open OBS.
2. From the top menu, select **Docks > Custom Browser Docks**.
3. Enter a name such as `ShoPro Control`.
4. Enter `https://shopro.live/shopro-app` as the URL.
5. Select **Apply**, then **Close**.
6. Sign in to ShoPro inside the new dock if prompted.
7. Open your show and switch to Run Mode.
8. Drag and resize the dock, or attach it to the OBS layout where it is easy to reach.

From the dock, you can follow the current and upcoming segments, start or end the show, advance the rundown, mark highlights, add a live topic, and control supported overlay visibility without leaving OBS. The controls available to you depend on your ShoPro account and role.

### Dock safety and workflow

- Treat the dock as a production control surface; an accidental click can change the live rundown or graphics.
- Decide who is responsible for advancing segments when multiple people have control access.
- Sign in and open the correct show before the production begins.
- Run a rehearsal and verify that dock actions update the correct browser sources.
- Keep enough width available for labels and controls to remain readable.
- Do not show the control dock in a display or window capture; it may contain scripts, notes, controls, or private links.
- If you use a shared computer, sign out of ShoPro after the production.

If the dock is missing after setup, open **Docks** in OBS and make sure **ShoPro Control** is checked. If it is blank or signed out, refresh the dock or reopen its custom dock settings and confirm the URL.

## Add a ShoPro graphic as a browser source

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

- Keep the ShoPro control dock separate from the scenes and sources sent to the audience.
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
