# Lumen Vision Remote Configuration

Remote configuration files for the Lumen Vision smart glasses app.

## Files

### `lumi-system-instruction.txt`
System instruction for Lumi 🌸 (Personal AI Assistant in Lumen Vision glasses).

**Usage:**
- Fetched by the Lumen Vision app on startup
- Cached for 5 minutes
- Falls back to hardcoded instruction if fetch fails

**To Update:**
1. Edit `lumi-system-instruction.txt`
2. Commit and push to `main` branch
3. Changes take effect on next app launch (or after 5 minute cache expires)

**Benefits:**
- Instant personality/instruction updates without rebuilding app
- No need for Jimmy to be home to deploy changes
- Works on all devices running Lumen Vision

## Architecture

**Hybrid Deployment Strategy:**
- **Remote Config** (this repo): System instructions, personality tweaks
- **TestFlight**: Code changes, new features, app updates

**URL:**
```
https://raw.githubusercontent.com/jimmylam-ai/lumen-vision-config/main/lumi-system-instruction.txt
```

---

*Maintained by Unc Lumen 💎*
