# Test Case: NoobTacoUI-Media (NTUI-media) Integration with LibSharedMedia

## Purpose
Validate that NoobTacoUI-Media (NTUI-media) assets (fonts, audio, graphics) are correctly registered and accessible via LibSharedMedia in the Midnight environment.

## Scope
- Font registration and usage
- Audio file registration and playback
- Graphics (statusbars, backgrounds, icons) registration and display

## Prerequisites
- NTUI-media addon installed and enabled
- LibSharedMedia library present and loaded
- Test environment: PTR, Beta, or Live

## Test Steps

### 1. Font Testing
- [ ] Confirm all NTUI-media fonts appear in the LibSharedMedia font list
- [ ] Select each NTUI-media font in a compatible addon (e.g., WeakAuras, Details!, ElvUI)
- [ ] Verify correct rendering in-game (no missing glyphs, correct style)
- [ ] Test fallback behavior if a font is missing

### 2. Audio File Testing
- [ ] Confirm all NTUI-media audio files are listed in LibSharedMedia
- [ ] Play each audio file via a compatible addon or script
- [ ] Verify correct playback (no distortion, correct file)
- [ ] Test fallback or error handling for missing files

### 3. Graphics Testing
- [ ] Confirm all NTUI-media statusbars, backgrounds, and icons are available in LibSharedMedia
- [ ] Select each graphic in a compatible addon (e.g., as a statusbar texture)
- [ ] Verify correct display (no corruption, correct image)
- [ ] Test fallback for missing/corrupt graphics

## Expected Results
- All NTUI-media assets are available and selectable via LibSharedMedia
- No errors or missing assets in-game
- Fallbacks work as expected if assets are missing

## Notes
- Document any issues with specific assets (file name, type, observed problem)
- Attach screenshots or logs as needed
