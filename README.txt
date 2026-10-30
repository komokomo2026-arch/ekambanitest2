EKAMBANI PWA - GitHub Pages upload package

UPLOAD
1. Extract this ZIP on your device.
2. Upload all extracted files and the icons folder to the ROOT of your GitHub repository.
3. GitHub repository > Settings > Pages > Deploy from a branch.
4. Select your main branch and /(root), then Save.
5. Wait for publishing and open the HTTPS GitHub Pages address.

INSTALL
- Icons: icon-192/512 (any), icon-maskable-192/512 (Android adaptive icons) and apple-touch-icon-180 (iPhone/iPad) must all be uploaded inside the icons folder.
- Android and Windows (Chrome, Edge and other compatible browsers): the Install button opens the browser's native install prompt immediately when the browser provides it. If it does not, the button shows the correct menu steps for that browser instead.
- iPhone/iPad: Safari > Share > Add to Home Screen > Add. The Install button shows these steps (iOS has no automatic install prompt).
- Firefox on computers and in-app browsers (Facebook, Instagram, WhatsApp, etc.) cannot install web apps; the button tells the user to open the page in Chrome, Edge or Safari.
- Not now hides the banner only for the current page load. Refresh/reopen shows it again.
- When opened as an installed app (standalone), the banner is hidden.

IMPORTANT LIMITATIONS
- The service worker caches only the GitHub Pages wrapper, manifest and icons.
- The Apps Script iframe is cross-origin. This wrapper cannot read/cache its internal data or make that app work offline. The embedded app still requires internet.
- Browsers decide whether to offer a native installation prompt. The banner remains available, but some browsers require installation through their own menu.
- iOS uses Safari's Add to Home Screen flow and does not provide the same automatic install prompt event.
- Cross-origin iframe server errors cannot all be detected by the wrapper.
- The original fullscreen request is retained. Browsers may reject automatic fullscreen without a user gesture.
