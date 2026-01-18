# Manual Addon Testing Workflow

This workflow outlines the standard procedure for verifying addon compatibility with **World of Warcraft: Midnight (12.0)**.

## 1. Preparation
- **Update the Addon**: Ensure you have the latest version installed (Retail or Beta version if available).
- **Enable Errors**: Ensure Lua errors are enabled in-game (`/console scriptErrors 1`) or use an error catching addon like *BugSack*/*BugGrabber*.
- **Tools**: Have the `addon-compatibility-tracker.md` open for logging.

## 2. Initial Load Check
1.  **Character Selection Screen**: 
    - Click **AddOns** in the bottom left.
    - Check if the addon is listed.
    - Check if it is marked "Out of Date" (Note: "Load out of date addons" should be checked).
2.  **Login**: Enter the world.
3.  **Chat Check**: Look for any "Addon Loaded" messages or immediate Lua errors in the chat window/error frame.

## 3. Functionality Verification
Perform the following checks based on the addon type:

### General Checks (All Addons)
- [ ] **Config Menu**: Can you open the addon's settings (Interface > Addons or minimap button)?
- [ ] **Slash Commands**: Do basic slash commands work (e.g., `/addon help`)?
- [ ] **Profiles**: Can you switch profiles without error?

### UI & Visuals
- [ ] **Positioning**: Are frames positioned correctly? (Midnight UI changes may offset elements).
- [ ] **Texture/Font Loading**: specific check for *NoobTacoUI-Media* or *SharedMedia* integration.
- [ ] **Scaling**: Does it scale correctly with UI scale changes?

### Mechanics (Specific Types)
- **Unit Frames**: Target self, friendly, hostile. Check cast bars.
- **Action Bars**: usable buttons, cooldown swipes, range coloring.
- **Maps**: Icons appear, tooltips work, zoom works.
- **Combat**: (If safe) Enter combat. Check for taint or errors during casting/actions.

## 4. Reporting & Logging
Update the `addon-compatibility-tracker.md` with your findings.

### Formatting the Entry
Copy the appropriate template and fill in the details:

**If Working:**
```markdown
- ✅ **Addon Name**
  [x] Works / [ ] Workaround / [ ] Will be later / [ ] Not working
  - *Status:* Works [Optionally add details like "in Midnight Alpha"]
  - *Notes:* [Any specific observations]
  - *Tested Date:* YYYY-MM-DD
  - *Version Tested:* x.y.z
  - *Last Tested:* YYYY-MM-DD
  - *Source:* User Testing
  - *Links:*
    - [CurseForge](...)
```

**If Issues Found:**
- Mark as `⚠️ Workaround` or `❌ Not working`.
- Detailed the issue in *Notes*.
- If a specific error occurs, save the stack trace in a separate file if needed, or summarize it in Notes.

## 5. Clean Up
- Disable the addon if it causes severe issues/crashes to continue testing others.
- Reset any temporary CVars if changed.
