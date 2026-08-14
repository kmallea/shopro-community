# Troubleshooting

## A shared view is not updating

- Confirm the owner and collaborator opened links for the same show.
- Refresh the shared page once.
- Check the aggregate connection summary.
- Verify that the role link has not been regenerated.
- Disable a VPN or restrictive browser extension temporarily.
- Confirm the network allows secure WebSocket connections.

## I cannot start the real show

An active test session may still exist. Return to Test Mode and exit or discard it, then try Run Mode again.

## Test data appeared in my real show

Current ShoPro versions isolate test timing, temporary topics, and highlights. Record the precise sequence—including whether the browser was refreshed or multiple operators were connected—and file a bug if any test data remains after exiting Test Mode.

## An OBS source is blank or stale

- Verify the complete source URL.
- Refresh the browser source cache in OBS.
- Confirm the source dimensions are not zero or cropped off-canvas.
- Open the URL in a current browser.
- Check HTTPS and WebSocket access.
- Confirm the correct ShoPro source is assigned to the show.

## A remote guest has no camera or microphone

- Confirm browser permission was granted.
- Select the correct device in the guest's browser settings.
- Close other applications using the device.
- Reconnect headphones or the audio interface before refreshing.
- Try a current Chromium-based browser.
- Check operating-system privacy permissions.

## Login does not persist

Enable cookies for `shopro.live`. Private browsing, aggressive privacy extensions, or automatic cookie deletion may prevent remembered login from working. Signing in again creates a new refresh session.

## Reporting a problem

Use the [bug report form](https://github.com/kmallea/shopro-community/issues/new?template=bug_report.yml) and include reproduction steps, browser, operating system, affected workflow, and sanitized screenshots. Never post credentials, shared-role links, or browser-source URLs.

