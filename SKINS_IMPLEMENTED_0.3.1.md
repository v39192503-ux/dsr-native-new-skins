# DSR Native 0.3.1 — Custom touch skin integration

- Integrated the fork's 29 PNG skin assets into `TouchControls` using Android `AssetManager`/`BitmapFactory`.
- Assets are decoded once when the overlay is created and cached; drawing reuses the bitmaps.
- Skin rendering replaces the previous code-drawn buttons and left stick visuals while preserving touch positions, hitboxes, multitouch, camera drag and controller input logic.
- Button mappings: A/B/X/Y, L/R, ZL/ZR, Minus/Plus, individual D-pad directions, L3 and LOCK; left stick uses base + nub normal/pressed variants.
- Pressed state uses supplied lit assets; face/menu/utility buttons use the ember ring overlay where no dedicated lit PNG exists.
- Camera remains direct touch-drag and is not given a skinned right stick.
- Tested on POCO F5: installed APK, opened the game Activity and captured a screen showing the custom skin in the character-creation screen. No crash observed in this short validation.

Build: `gradle assembleDebug --no-daemon`
APK: `DSRNative_0.3.1_Skins_Debug.apk`
