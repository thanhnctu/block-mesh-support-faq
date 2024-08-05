# BlockMesh Network - Support FAQ

## Debug Connection Issues

### Step 1
1. Logout and re-login into the extension.
2. Wait for 180 seconds.
3. Check status again (refresh dashboard).

### Step 2 - If `Step 1` failed
1. Go to `manage extensions` menu in `Chrome`.
2. Click on BlockMesh Network extension `service worker`.
3. Check the `console` and `network` tabs for errors.
4. If there are errors, screenshot them.
5. Check the output of commands `await chrome.storage.sync.get("blockmesh_api_token")` and `await chrome.storage.sync.get("email")`.
6. Please include the extension `version` in the email.
7. Please send details from #4 #5 #6  to `support@blockmesh.xyz`.
